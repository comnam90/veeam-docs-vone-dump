---
title: "Updating and Renewing License"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/update_license.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Updating and Renewing License


When your Veeam ONE license nears expiration, you can renew it to extend its term and keep receiving product updates and technical support. After you renew the license, update it to install the renewed key.

|  |
| --- |
| Note: |
| To prevent potential conflicts with license updates, ensure that the date and time settings on the machines hosting Veeam ONE components are synchronized with the NTP (Network Time Protocol) servers within your organization. |

Renewing License

To renew the license:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click License Information.
3. At the top of the License tab, click Renew.

The Veeam license renewal page opens in your web browser. Follow the instructions on the page to request a license renewal.

After Veeam processes the renewal, update the license to install the renewed key, either manually or automatically.

Updating License Manually

You can update the license from the Veeam License Update Server manually on demand. When you update the license manually, Veeam ONE connects to the Veeam License Update Server, downloads a new license from it (if the license is available), and displays the updated license information for review.

To update the license:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click License Information.
3. On the License tab, click Update.

Veeam ONE will connect to the Veeam License Update Server, download the new license (if available), and display the updated license information on the License tab.

1. Click Save to apply the changes.

Updating License Automatically

You can instruct Veeam ONE to update the license automatically. License auto update is available for all license types. It is enabled by default for Community Edition, Evaluation, and NFR licenses that have a Support ID; for Evaluation and NFR licenses without a Support ID, it is disabled by default and can be enabled manually. Automatic license update removes the need to download and install the license manually each time you purchase a license extension. If the automatic update option is enabled, Veeam ONE proactively communicates with the Veeam License Update Server to obtain and install a new license before the current license expires.

How Automatic License Update Works

To update the license automatically, Veeam ONE performs the following actions:

1. After you enable automatic license update, Veeam ONE starts sending requests to the Veeam License Update Server on the web (one.butler.veeam.com) and checks if a new license key is available. Veeam ONE sends requests once a week. Communication with the Veeam License Update Server is performed over the HTTPS protocol.
2. Seven days before the expiration date of the current license, Veeam ONE starts sending requests once a day.
3. When a new license key becomes available, Veeam ONE automatically downloads it and installs on the Veeam ONE server.

Automatic license update can complete with the following results:

* Operation is successful — a new license key is generated, downloaded and installed on the Veeam ONE server.
* A new license is not required — the currently installed license key does not need to be updated.
* Veeam License Update Server has failed to generate a new license — such situation can occur due to an error on the Veeam License Update Server side.
* Veeam ONE has received an invalid answer — such situation can occur due to connectivity issues between the Veeam License Update Server and Veeam ONE server.

Automatic Update Retries

If Veeam ONE fails to update the license, it triggers the Veeam ONE license update failure alarm, and retries to update the license.

Veeam ONE retries to update the license key in the following way:

* If Veeam ONE fails to establish a connection to the Veeam License Update Server, retry takes place every 60 minutes.
* If Veeam ONE establishes a connection but there occurs a general license key generation error, the retry takes place every 24 hours.

The retry period ends one month after the license expiration date or the support expiration date (whichever is earlier). The retry period is equal to the number of days in the month of license expiration. For example, if the license expires in January, the retry period will be 31 days. If the license expires in April, the retry period will be 30 days.

Enabling Automatic License Update

By default, automatic license update is disabled. To enable automatic license updates:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the top right corner of the Veeam ONE Web Client window, click Configuration.
2. In the configuration menu on the left, click License Information.
3. On the License tab, select the Update license automatically (enables usage reporting) check box.
4. Click Save.

|  |
| --- |
| Note: |
| Enabling license auto update activates [License Usage Statistics](automatic_usage_logging.md). You cannot use license auto update without automatic usage reporting. |

Page updated 2026-07-24

