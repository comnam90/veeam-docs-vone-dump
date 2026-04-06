---
title: "Changing Veeam ONE Service Account"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/change_service_account.html"
last_updated: "9/30/2025"
product_version: "13.0.1.6168"
---

# Changing Veeam ONE Service Account


You can change Veeam ONE service account or the service account password that you provided during the product installation. For example, changing Veeam ONE service account properties can be required if you use a domain account as the Veeam ONE service account. When you update the domain account password, you must manually update the service account password for Veeam ONE.

To change the Veeam ONE service account or service account password:

1. Log on as Administrator to the machine where the Veeam ONE Server component is installed.
2. Change accounts of Veeam ONE Caching Service, Veeam ONE Monitoring Service, Veeam ONE Error Reporting Service, Veeam ONE Reporting Service and Veeam Analytics service:

1. Click Start, go to Programs > Administrative Tools, and then click Services.
2. Right-click Veeam ONE Monitoring Service and choose Stop.
3. Right-click Veeam ONE Monitoring Service, choose Properties and open the Log on tab.
4. In the This account filed, specify the user name of the service account.
5. In the Password and Confirm password fields, type a password of the service account.
6. Click OK.
7. Repeat steps a–f for Veeam ONE Reporting Service, Veeam Analytics service, Veeam ONE caching Service and Veeam ONE Error Reporting Service.

1. Start Veeam ONE Caching Service, Veeam ONE Monitoring Service, Veeam ONE Error Reporting Service, Veeam ONE Reporting Service and Veeam Analytics service:

1. Click Start, go to Programs > Administrative Tools, and then click Services.
2. Right-click the necessary service and choose Start.

|  |
| --- |
| Important! |
| If you want to use Local System as the service account, consider the following:   * SQL Server Authentication is required for the account used to connect to the Microsoft SQL Server hosting the Veeam ONE database.   For details on modifying database connection settings, see [Database](utility_general.md).   * You cannot install the license using the POST /license/install method of the Veeam ONE REST API. |

Other Ways to Change Service Account

To change Veeam ONE service account, you can also perform the following steps:

1. Uninstall Veeam ONE.
2. Re-install Veeam ONE and specify a new service account during installation.

Note that when you re-install Veeam ONE, you must point it to the existing Veeam ONE database.


