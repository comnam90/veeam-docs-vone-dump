---
title: "Veeam ONE Settings Utility"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/appendix.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Veeam ONE Settings Utility


The Veeam ONE Settings utility allows you to change configuration of the Veeam ONE software components.

|  |
| --- |
| Note: |
| The Veeam ONE Settings utility must be used only under the guidance of Veeam Support. It is strongly recommended that you obtain detailed instructions from the Veeam Support team before changing any configuration settings in your Veeam ONE deployment. |

To run the Veeam ONE Settings utility:

1. Log in to Veeam ONE Client under account with Local Administrator permissions on the machine where Veeam ONE Server component is installed.

For details, see [Accessing Veeam ONE Components](access.md).

|  |
| --- |
| Note: |
| If you use Microsoft Windows authentication to connect to Microsoft SQL Server, make sure that the user under which you launch Veeam ONE Settings utility has sufficient permissions to access Veeam ONE database. Otherwise the Retention Policy Period and Scalability settings in the utility will be unavailable. |

1. In the main menu, click Settings > Server Settings.

Alternatively, press [CTRL + S] on the keyboard.

1. Open the Other tab.
2. In the Support utility section, click Launch.

This section describes configuration settings that you can change using the Veeam ONE Settings utility.

In This Section

* [General Settings](utility_general.md)
* [Veeam ONE Server Settings](utility_monitor.md)
* [Veeam ONE Web Settings](utility_reporter.md)
* [Scalability](utility_deployment.md)
* [Exporting Logs](utility_export_logs.md)


