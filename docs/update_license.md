---
title: "Updating License"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/update_license.html"
last_updated: "5/12/2025"
product_version: "13.0.1.6168"
---

# Updating License


When the license expires, you can update it from the Veeam licensing server. You can use the following methods to update Veeam ONE license:

* Update the license manually
* Update the license automatically

|  |
| --- |
| Note: |
| To prevent potential conflicts with license updates, ensure that the date and time settings on the machines hosting Veeam ONE components are synchronized with the NTP (Network Time Protocol) servers within your organization. |

Updating License Manually

You can update the license from the Veeam License Update Server manually on demand. When you update the license manually, Veeam ONE connects to the Veeam License Update Server, downloads a new license from it (if the license is available), and installs it on the Veeam ONE server.

To update the license:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. In the main menu, click License.
2. In the License Information window, navigate to the License tab.
3. Click Update.

Veeam ONE will connect to the Veeam licensing server, download the new license from it (if available), install it on the Veeam ONE server, and display a dialog box with the license update result.

1. Click Save to acknowledge the result and close the dialog box.

Updating License Automatically

You can instruct Veeam ONE to update the license automatically. License auto-update is available for all types of licenses and is mandatory for Free licenses (Community Edition, Evaluation, NFR). Automatic license update removes the need to download and install the license manually each time when you purchase the license extension. If the automatic update option is enabled, Veeam ONE proactively communicates with the Veeam License Update Server to obtain and install a new license before the current license expires.

How Automatic License Update Works

To update the license automatically, Veeam ONE performs the following actions:

1. After you enable automatic license update, Veeam ONE starts sending requests to the Veeam License Update Server on the web (one.butler.veeam.com) and checks if a new license key is available. Veeam ONE sends requests once a week. Communication with the Veeam License Update Server is performed over the HTTPS protocol.
2. Seven days before the expiration date of the current license, Veeam ONE starts sending requests once a day.
3. When a new license key becomes available, Veeam ONE automatically downloads it and installs on the Veeam ONE server.

Automatic license update can complete with the following results:

* Operation is successful. A new license key is successfully generated, downloaded and installed on the Veeam ONE server.
* A new license is not required. The currently installed license key does not need to be updated.
* Veeam License Update Server has failed to generate a new license. Such situation can occur due to an error on the Veeam License Update Server side.
* Veeam ONE has received an invalid answer. Such situation can occur due to connectivity issues between the Veeam License Update Server and Veeam ONE server.

Automatic Update Retries

If Veeam ONE fails to update the license, it triggers the Veeam ONE license update failure alarm, and retries to update the license.

Veeam ONE retries to update the license key in the following way:

* If Veeam ONE fails to establish a connection to the Veeam License Update Server, retry takes place every 60 minutes.
* If Veeam ONE establishes a connection but there occurs a general license key generation error, the retry takes place every 24 hours.

The retry period ends one month after the license expiration date or the support expiration date (whichever is earlier). The retry period is equal to the number of days in the month of license expiration. For example, if the license expires in January, the retry period will be 31 days. If the license expires in April, the retry period will be 30 days.

Enabling Automatic License Update

By default, automatic license update is disabled. To enable automatic license updates:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. In the main menu, click License.
2. In the License Information window, on the License tab, select the Update license automatically (enables usage reporting) check box.
3. Click Save.

|  |
| --- |
| Note: |
| * Enabling license auto update activates [License Usage Statistics](automatic_usage_logging.md). You cannot use license auto update without automatic usage reporting. * License auto-update is enabled by default for Free licenses (Community Edition, Evaluation, NFR) and cannot be disabled. |


