---
title: "Alarm Rules for Veeam Backup for Microsoft 365"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbm_alarm_rules.html"
last_updated: "11/5/2024"
product_version: "13.0.1.6168"
---

# Alarm Rules for Veeam Backup for Microsoft 365


Veeam ONE offers the following types of alarm rules for Veeam Backup for Microsoft 365 infrastructure objects.

Veeam Backup for Microsoft 365 Server

Veeam Backup for Microsoft 365 Server

| Rule Type | Description |
| Job disabled | An alarm is triggered if the time during which a job was disabled has exceeded the specified threshold. |
| Job status | An alarm is triggered if the job status is equal or not equal to the specified value. |
| Event-based rule | An alarm is triggered if some Veeam Backup for Microsoft 365 event is generated for the backup server. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Organization without backups | An alarm is triggered if no backups were created for a Microsoft 365 organization during the specified RPO interval. |
| Power or connection state changes | An alarm is triggered if the state of Veeam Backup for Microsoft 365 server is equal or not equal to the specified value (for example, if connection to the server is lost). |
| Restore activity | An alarm is triggered if Veeam Backup for Microsoft 365 restore session is initiated for the defined object type. |
| Unusual job duration | An alarm is triggered if duration of a job session is above specified percentage based on the set of latest job sessions. |
| Veeam Backup for Microsoft 365 Service state | An alarm is triggered if the Veeam Backup for Microsoft 365 Service state is equal or not equal to the specified value. |

Backup Proxy

Backup Proxy

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some Veeam Backup for Microsoft 365 event is generated for the proxy server. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Power or connection state changes | An alarm is triggered if the state of proxy server is equal or not equal to the specified value (for example, if connection to the proxy server is lost). |
| Maintenance mode | An alarm is triggered if backup proxy maintenance mode is enabled. |

Backup Repository

Backup Repository

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the repository. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Backup repository is running out of free space | An alarm is triggered if free space on the repository is above or below the specified threshold value. You can select to specify the free space threshold as an absolute value or a relative value. For example, an alarm is triggered if the storage space is below 10 GB or 15% of total space. |


