---
title: "Connecting Veeam Backup & Replication Servers"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_server_connect.html"
last_updated: "4/29/2026"
product_version: "13.0.1.6168"
---

# Connecting Veeam Backup & Replication Servers


To collect data about your backup infrastructure and data protection operations, you must configure connections to Veeam Backup & Replication servers in Veeam ONE Web Client. You can connect the following types of servers:

* Veeam Backup & Replication server to monitor standalone backup servers
* Veeam Backup Enterprise Manager to monitor all backup servers federated under Veeam Backup Enterprise Manager

|  |
| --- |
| Note: |
| * Before you connect a Veeam Backup & Replication server to Veeam ONE check that product licenses are compatible. For details on license compatibility, see [Compatibility with Veeam Backup & Replication Licenses](license_types.md#compatibility). * To install the Veeam Analytics Service package on Veeam Software Appliance, you must enable remote data collection in the Host Management Interface. For more information, see section [Enabling Remote Data Collection](https://helpcenter.veeam.com/docs/vbr/userguide/hmc_configure_infrastructure.html?ver=13#enabling-remote-data-collection) of the Veeam Backup & Replication User Guide. * Veeam Backup & Replication servers can optionally be added to Veeam ONE through manual installation of Veeam Analytics service. For details on manual installation of Veeam Analytics service, see [Veeam Analytics Service](veeam_analytics_service.md#manual_installagent). |

To configure a connection to a Veeam Backup & Replication server, take the following steps.

1. [Launch the Add Server wizard](backup_server_launch.md).
2. [Choose server type](backup_server_type.md).
3. [Specify server name and role](backup_server_name.md).
4. [Specify Veeam Analytics service deployment credentials](backup_server_credentials.md).
5. [Specify backup monitoring credentials](backup_monitor_credentials.md)
6. [Review connection settings](backup_server_review.md).


