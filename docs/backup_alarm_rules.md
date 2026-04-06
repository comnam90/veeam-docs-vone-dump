---
title: "Alarm Rules for Veeam Backup & Replication"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_alarm_rules.html"
last_updated: "10/24/2025"
product_version: "13.0.1.6168"
---

# Alarm Rules for Veeam Backup & Replication


Veeam ONE offers the following types of alarm rules for Veeam Backup & Replication infrastructure objects.

Enterprise Manager

Enterprise Manager

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the Veeam Backup Enterprise Manager. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Power or connection state changes | An alarm is triggered if the state of Veeam Backup Enterprise Manager is equal or not equal to the specified value (for example, if connection to the Enterprise Manager is lost). |

Backup Server

Backup Server

| Rule Type | Description |
| CDP VM SLA % | An alarm is triggered if CDP policy SLA is below the specified threshold. |
| Backup Copy RPO | An alarm is triggered if no backup copy VM restore points were created during the specified period. |
| Cloud instance RPO | An alarm is triggered if no cloud instance restore points were created during the specified period. |
| Incremental backup size | An alarm is triggered if size of one or more increments has exceeded the specified threshold. |
| Disabled job | An alarm is triggered if the time during which a job was disabled has exceeded the specified threshold. |
| Job/Policy status | An alarm is triggered if the job or policy status is equal or not equal to the specified value. |
| Plug-in backup data collection failure | An alarm is triggered if the Veeam ONE server fails to collect plug-in backup data. |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the backup server. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Job duration exceeded the allowed time period | An alarm is triggered if duration of a job exceeds the threshold specified in minutes. |
| Power or connection state changes | An alarm is triggered if the state of Veeam Backup & Replication server is equal or not equal to the specified value (for example, if connection to the backup server is lost). |
| Unusual job duration | An alarm is triggered if duration of a job session is above specified percentage based on the set of latest job sessions. |
| Backup security and compliance | An alarm is triggered if the defined best practices statuses are detected. |
| Disabled malware detection | An alarm is triggered if disabled malware is detected. |
| Potential malware activity | An alarm is triggered if suspicious or infected malware is detected on your data. |
| VM Backup RPO (oVirt KVM, Proxmox, AHV) | An alarm is triggered if no VM (oVirt KVM, Proxmox, AHV) restore points were created during the specified period. |

Repository

Repository

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the repository. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Immutability state | An alarm is triggered if immutability is disabled for repositories or repository extents. |
| Out-of-date state | An alarm is triggered if Veeam Backup & Replication software components installed on the repository server are out of date. |
| Power or connection state changes | An alarm is triggered if the state of the backup repository is equal or not equal to the specified value (for example, if connection to the repository is lost). |
| Repository server is running out of free space | An alarm is triggered if free space on the repository is above or below the specified threshold value. You can select to specify the free space threshold as an absolute value or a relative value. For example, an alarm is triggered if the storage space is below 10 GB or 15% of total space. |

Proxy

Proxy

| Rule Type | Description |
| CDP Proxy Cache Usage | An alarm is triggered if the CDP cache usage is above the specified threshold. |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the proxy server. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Out-of-date state | An alarm is triggered if Veeam Backup & Replication software components installed on the proxy server are out of date. |
| Power or connection state changes | An alarm is triggered if the state of proxy server is equal or not equal to the specified value (for example, if connection to the proxy server is lost). |

WAN Accelerator

WAN Accelerator

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the WAN accelerator. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Out-of-date state | An alarm is triggered if Veeam Backup & Replication software components installed on the WAN accelerator server are out of date. |
| Power or connection state changes | An alarm is triggered if the state of the WAN accelerator is equal or not equal to the specified value (for example, if connection to the WAN accelerator is lost). |

Tape Server

Tape Server

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the tape server. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Out-of-date state | An alarm is triggered if Veeam Backup & Replication software components installed on the tape server are out of date. |
| Power or connection state changes | An alarm is triggered if the state of the backup repository is equal or not equal to the specified value (for example, if connection to the server is lost). |

Cloud Repository

Cloud Repository

| Rule Type | Description |
| Cloud repository lease expiration | An alarm is triggered if cloud repository lease time will expire in the specified number of days. |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the cloud repository. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Number of VMs stored in repository | An alarm is triggered if the number of VMs stored in the backup repository has exceeded the specified threshold. |
| Repository server is running out of free space | An alarm is triggered if free space on the repository is above or below the specified threshold value. You can select to specify the free space threshold as an absolute value (for example, if the storage space should not fall below 10 GB) or a relative value (for example, if the free space should not fall below 15% of total space). |

Cloud Gateway

Cloud Gateway

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the cloud gateway. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Out-of-date state | An alarm is triggered if Veeam Backup & Replication software components installed on the cloud gateway server are out of date. |
| Power or connection state changes | An alarm is triggered if the state of the backup repository is equal or not equal to the specified value (for example, if connection to the cloud gateway is lost). |

Enterprise Application

Enterprise Application

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some Veeam Backup & Replication event is generated for the application. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Application backup RPO | An alarm is triggered if no application database backups were created during the specified period. |


