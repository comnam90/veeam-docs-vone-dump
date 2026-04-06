---
title: "Configuring SSRS Server Settings"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/configure_ssrs_server_settings.html"
last_updated: "9/17/2025"
product_version: "13.0.1.6168"
---

# Configuring SSRS Server Settings


When you report on a large virtual infrastructure, you may experience slowdowns with generating reports. In this case, you can integrate an SSRS server with Veeam ONE Web Client and use this SSRS server as an alternative to the default Veeam ONE report viewer.

|  |
| --- |
| Note |
| SSRS server is not used for generating Veeam Backup & Replication and Veeam Backup for Microsoft 365  reports that work with Veeam ONE version 13's new report engine. Reports that currently use the legacy engine including VMware, Hyper-V and vCD still require SSRS server configuration. |

To configure SSRS server settings you must have the following permissions:

* System User role in SSRS site settings
* Content Manager role in SSRS Home folder settings
* User mapping to Veeam ONE database with public role
* Select and Execute permissions on Veeam ONE database

You can specify access settings to the Microsoft SQL Reporting Services server that will be used for integration with Veeam ONE Web Client:

1. Open Veeam ONE Web Client.
2. At the top right corner of the Veeam ONE Web Client window, click Configuration.
3. In the configuration menu on the left, click Reporting Settings.
4. In the Microsoft SQL Server Reporting Services (SSRS) Server Settings section, select the Use SSRS server for generating reports check box.
5. In the Server URL field, enter the address of the SSRS hosting server.

The URL must be specified in the following format: https://servername:port/virtualdirectory. To check if this URL is correct, launch the Reporting Services Configuration Manager and check the Web Service URL section.

1. Specify a user name and a password to connect to the SSRS server.

The user name must be specified in the DOMAIN\USERNAME format.

1. To verify SSRS server settings, click Test Connection. Veeam ONE Web Client will display verification results on a summary screen.
2. Click Save to save SSRS server settings.

[![Configure SSRS Server Settings](images/report_branding_02.webp)](images/report_branding_02.webp "Configure SSRS Server Settings")


