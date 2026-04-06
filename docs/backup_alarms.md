---
title: "Veeam Backup & Replication Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_alarms.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Veeam Backup & Replication Alarms


Veeam ONE includes a set of alarms monitor the efficiency of Veeam Backup & Replication data protection in the virtual environment.

Predefined data protection alarms are configured to warn you about events or issues that can cause loss of data or prevent Veeam Backup & Replication infrastructure from functioning properly:

* Connectivity issues and inability of backup infrastructure components to communicate with each other
* State of Veeam Backup & Replication software installed on backup infrastructure components
* Failing jobs or jobs finished with warnings
* Configuration issues, such as fast decreasing space on backup repositories or cloud repositories
* Long-running jobs that exceed the backup window
* Product license and prepaid support contract

To view the list of data protection alarms:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Veeam Backup & Replication.
2. In the inventory pane, select the necessary backup infrastructure node.
3. Open the Alarms tab.

On the Alarms dashboard, you can view triggered alarms, track alarm history, resolve and acknowledge alarms and perform other actions. For details on available actions, see [Working with Triggered Alarms](triggered_alarms.md).

[![Data Protection Alarms](images/monitoring_vbr_alarms.webp)](images/monitoring_vbr_alarms.webp "Data Protection Alarms")


