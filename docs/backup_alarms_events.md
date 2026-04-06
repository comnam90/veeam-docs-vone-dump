---
title: "Veeam Backup & Replication Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_alarms_events.html"
last_updated: "12/11/2025"
product_version: "13.0.1.6168"
---

# Veeam Backup & Replication Alarms


This section describes predefined alarms for Veeam Backup & Replication infrastructure components.

Enterprise Manager

Enterprise Manager

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Veeam Backup Enterprise Manager connection failure | State does not equal Connected. | Error | Automatic | Veeam ONE failed to connect to Veeam Backup Enterprise Manager. |

Veeam Backup & Replication Server

Veeam Backup & Replication Server

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Agent backup job state | State of an agent backup job equals Warning. | Warning | Automatic | One or more computers failed to back up successfully. |
| State of an agent backup job equals Failed. | Error |
| Agent backup policy session state | State of a backup policy session equals Warning. | Warning | Automatic | One or more computers failed to back up successfully. |
| State of a backup policy session equals Failed. | Error |
| Application backup policy state | State of a backup policy session equals Warning. | Warning | Automatic | One or more application databases failed to back up successfully. |
| State of a backup policy session equals Failed. | Error |
| Backup Copy Job exceeded data transfer window | Based on event | Error | Manual | One or more backup copy jobs exceeded defined window, and data transfer between source and target backup repositories has been stopped. |
| Backup Copy job state | State of an backup copy job equals Warning. | Warning | Automatic | One or more objects could not be successfully copied from the backup repository. |
| State of an backup copy job equals Failed. | Error |
| Backup Copy RPO | Restore point copy is missing according to job schedule. | Error | Automatic | One or more backups was not successfully copied to the secondary repository within the defined RPO interval. |
| Backup Server Failed Logon Attempt | Based on event | Error | Manual | Authentication of Veeam Backup & Replication service failed during logon. |
| Based on event 44002 Veeam MP | Error | Manual |
| Backup Server Successful Logon | Based on event 44000 Veeam MP | Information | Automatic | Successful authorization attempt completed on Veeam Backup & Replication. |
| 44003 Veeam MP | Information | Automatic |
| Backup Server security & compliance state | Backup security & compliance state is not implemented. | Error | Automatic | Security & compliance check finished with warning or error. |
| Backup security & compliance state is unable to detect. | Warning |
| Backup security & compliance state is not checked. | Warning |
| Cloud instance RPO | No cloud instance protection type was created for more than 24 hours. | Warning | Automatic | No cloud instance protection type was created within the defined RPO interval. |
| Job disabled | Job is disabled for more than 12 hours. | Warning | Automatic | Job stays in the disabled state for a longer time than configured in the alarm threshold. |
| Backup job failed to create storage snapshot | Based on event VeeamBpJobFailedToCreateStorageSnapshotEvent. | Warning | Manual | Integrated storage failed to create storage snapshot initiated by Veeam backup job. |
| Backup job state | State of a backup job equals Warning. | Warning | Automatic | Backup job reported either an error or a warning. |
| State of a backup job equals Failed. | Error |
| State of a Nutanix backup job equals Warning. | Warning |
| State of a Nutanix backup job equals Failed. | Error |
| CDP SLA Compliance | SLA decreases to 95% for 5 minutes. | Warning | Automatic | SLA % of one or more workloads processed by CDP policy has dropped below threshold. |
| SLA decreases to 75% for 5 minutes. | Error |
| Cloud backup policy session state | Status of a cloud backup policy session equals Warning. | Warning | Automatic | Policy finished with warning or error. |
| Status of a cloud backup policy session equals Error. | Error |
| File backup job state | State of a file backup job equals Warning. | Warning | Automatic | File backup job finished with warning or error. |
| State of a file backup job equals Failed. | Error |
| File copy job state | State of a file copy job equals Warning. | Warning | Manual | One or more files failed to be transferred to the destination folder. |
| State of a file copy job equals Failed. | Error |
| Job exceeded backup window | Based on event VeeamBpJobWindowExceededEvent. | Error | Manual | One or more jobs exceeded allowed backup window and has been terminated. |
| License expiration date | Based on event VeeamBackupServerLicenseExpiration. | Warning | Automatic | Veeam Backup & Replication license expired. |
| Based on event VeeamBackupServerLicenseChanged. | Resolve |
| Based on event VeeamBackupServerLicenseExpirationResolve. | Resolve |
| Maximum allowed job duration | Job duration is more than 480 minutes. | Error | Manual | Job has exceeded its maximum allowed execution time. |
| Job duration is more than 120 minutes. | Warning |
| Object storage backup job state | Object storage backup job equals failed. | Error | Automatic | One or more unstructured data items in the object storage backup were not successfully backed up. |
| Object storage backup job equals warning. | Warning |
| Potential malware in backups | One or more files detected as infected with malware. | Error | Automatic | One or more files with suspicious or infected malware detection. |
| One or more files detected with potential suspicious malware infection. | Warning |
| Plug-in backup data collection failure | Plug-in backup data collection failed due to connection loss for more than 5 minutes. | Error | Automatic | Veeam ONE server failed to collect plug-in backup data provided by Veeam Backup & Replication. |
| Quick Migration job state | Based on event VeeamBpQMigrationSessionWarningEvent. | Warning | Automatic | One or more VMs failed to migrate to another host. |
| Based on event VeeamBpQMigrationSessionErrorEvent. | Error |
| Replication job state | State of a replication job equals Warning. | Warning | Automatic | One or more VMs failed to replicate successfully. |
| State of a replication job equals Failed. | Error |
| Restore activity | Based on event 290 Veeam MP. | Information | Automatic | Restore session initiated. |
| Based on event 40290 Veeam MP. |
| Support expiration date | Based on event VeeamBackupServerLicenseSupportExpiration. | Warning | Automatic | Veeam Backup & Replication prepaid support contract expired. |
| Based on event VeeamBackupServerLicenseChanged. | Resolve |
| Based on event VeeamBackupServerLicenseSupportExpirationResolved. | Resolve |
| SureBackup job state | State of a SureBackup job equals Warning. | Warning | Automatic | One or more VMs could not be successfully verified. |
| State of a SureBackup job equals Failed. | Error |
| Suspicious incremental backup size | One of 3 last job increment sizes is above 150% of configured threshold. | Warning | Automatic | The size of the recently created incremental restore point is significantly different from the previously created ones.  For Oracle RMAN backup jobs, Veeam ONE analyzes only the differential level 1 backups. |
| One of 3 last job increment sizes is above 200% of configured threshold. | Error |
| One of 3 last job increment sizes is below 80% of configured threshold. | Warning |
| One of 3 last job increment sizes is below 70% of configured threshold. | Error |
| Tape job state | Status of the file to tape backup job equals Warning. | Warning | Manual | One or more VMs, computers or unstructured data items failed to be transferred to the tape device. |
| Status of the file to tape backup job equals Failed. | Error |
| Status of the backup to tape job equals Warning. | Warning |
| Status of the backup to tape job equals Failed. | Error |
| Database log backup job state | Microsoft SQL server log backup job completed with warning. | Warning | Automatic | Database transaction logs have not been backed up successfully. |
| Microsoft SQL server log backup job failed. | Error |
| Oracle Database log backup job completed with warning. | Warning |
| Oracle Database log backup job failed. | Error |
| PostgreSQL log backup job completed with warning. | Warning |
| PostgreSQL log backup job failed. | Error |
| Enterprise application log backup job completed with warning. | Warning |
| Enterprise application log backup job failed. | Error |
| Unusual job duration | Job duration is above 150% of average time interval. | Warning | Automatic | Job duration is above usual values among the set of job sessions. |
| Job duration is above 200% of average time interval. | Error |
| Veeam Backup & Replication HA cluster created | Based on event 43000 Veeam MP | Information | Automatic | High availability cluster was created. |
| Veeam Backup & Replication HA cluster disassembled | Based on event 43002 Veeam MP | Information | Automatic | High availability cluster was disassembled. |
| Veeam Backup & Replication HA cluster primary node state | Based on event VeeamBpHaClusterOfflineEvent | Error | Automatic | Primary node of high availability cluster stopped communicating with Veeam ONE. |
| Based on event VeeamBpHaClusterOfflineResolvedEvent | Resolve | Automatic | Communication with primary node of high availability cluster successfully restored. |
| Based on event VeeamMonitorServicesStarted | Resolve | Automatic |
| Veeam Backup & Replication HA cluster secondary node state | Based on event 43003 Veeam MP | Error | Automatic | Veeam Backup & Replication HA secondary node state is offline. |
| Based on event 43003 Veeam MP | Resolve | Automatic | Veeam Backup & Replication HA secondary node state is online. |
| Veeam Backup & Replication HA cluster failover state | Based on event 43004 Veeam MP | Information | Automatic | High availability cluster failover activity initiated. |
| Veeam Backup & Replication HA cluster switchover state | Based on event 43006 Veeam MP | Information | Automatic | High availability cluster switchover activity successfully completed. |
| Veeam Backup & Replication Server connection failure | State does not equal Connected. | Error | Automatic | Connection to Veeam Backup & Replication server failed. |
| Veeam Broker Service state | Based on event VeeamBackupServerBrokerServiceDownEvent. | Warning | Automatic | Veeam Broker Service that interacts with virtual infrastructure to collect and cache its topology is not started and not working properly. |
| Based on event VeeamBackupServerBrokerServiceDownEvent. | Resolve |
| Based on event VeeamBackupServerBrokerServiceDownEvent. | Resolve |
| Veeam malware detection activity state | Disabled malware detection. | Error | Automatic | This event is triggered when inline entropy or file system activity analysis settings are disabled. |
| Veeam malware detection exclusions change tracking | Based on event 42260 Veeam MP. | Error | Manual | A workload was added to or removed from the malware detection exclusions list. |
| Based on event 42270 Veeam MP. | Error |
| Veeam malware detection change tracking | Based on event VeeamMalwareInlineEntropyAnalysisEnabled. | Warning | Manual | Events are triggered when malware scan settings are changed. |
| Based on event VeeamMalwareInlineEntropyAnalysisDisabled. | Warning |
| Based on event VeeamMalwareSensitivityDecreased. | Warning |
| Based on event VeeamMalwareSensitivityIncreased. | Warning |
| Based on event VeeamUpdateMalwareDefinitionsAutomaticallyDisabled. | Warning |
| Based on event VeeamUpdateMalwareDefinitionsAutomaticallyEnabled. | Warning |
| Based on event VeeamMalwareIncludedExtensionsListChanged. | Warning |
| Based on event VeeamMalwareExcludedExtensionsListChanged. | Warning |
| Based on event VeeamMalwareFileSystemActivityAnalysisDisabled. | Warning |
| Based on event VeeamMalwareFileSystemActivityAnalysisEnabled. | Warning |
| VM Backup RPO (oVirt KVM, Proxmox VE, Nutanix AHV) | No VM backups were created for more than 24 hours. | Warning | Automatic | This VM has not been backed up within the defined RPO (Recovery Point Objective) interval. |

Repository

Repository

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Backup repository connection failure | State equals Not accessible for more than 5 minutes. | Error | Automatic | Veeam Backup & Replication server lost connection to the Microsoft Windows backup repository. |
| State equals Partially accessible for more than 5 minutes. | Warning |
| Backup repository free space | Free space is below 5%. | Error | Automatic | Backup repository is low on free space. |
| Free space is below 10%. | Warning |
| Backup repository version is out-of-date | Component version mismatch. | Warning | Automatic | Veeam backup repository version does not match the version of Veeam Backup & Replication server. |
| Backup repository ReFS data integrity issue | Based on event 133 ReFS. | Warning | Manual | ReFS-formatted volume of a backup repository experienced a data integrity issue. |
| Based on event 135 ReFS. |
| Based on event 136 ReFS. |
| Immutability state | Immutability is disabled. | Warning | Automatic | The immutability setting is turned off on one or several backup repositories or scale-out backup repository extents. |
| Immutability change tracking | Based on event VeeamImmutabilityIntervalDaysDecreased. | Warning | Manual | The configured immutability period has been changed on one or several backup repositories or scale-out backup repository extents. |
| Based on event VeeamImmutabilityIntervalDaysIncreased. |
| Based on event VeeamImmutabilityIntervalDaysEnabled. |
| Scale-out backup repository data transfer session state | Scale-out backup repository data transfer session completed with warning. | Warning | Automatic | Scale-out backup repository offload, download, archiving or retrieval data transfer session finished with warning or failed. |
| Scale-out backup repository data transfer session failed. | Error |

Proxy

Proxy

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Backup proxy connection failure | State does not equal Accessible for more than 5 minutes. | Error | Automatic | Veeam Backup & Replication server lost connection to the backup proxy server. |
| Backup proxy version is out-of-date | Component version mismatch. | Warning | Automatic | Veeam backup proxy version does not match the version of Veeam Backup & Replication server. |
| CDP proxy cache usage | CDP cache usage is above 50% | Warning | Automatic | CDP proxy cache usage has reached the configured threshold. |
| CDP cache usage is above 75% | Error |

WAN Accelerator

WAN Accelerator

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| WAN accelerator connection state | State does not equal Accessible for more than 5 minutes. | Error | Automatic | Veeam Backup & Replication server lost connection to the WAN accelerator |
| WAN accelerator version is out-of-date | Component version mismatch. | Warning | Automatic | Veeam WAN accelerator version does not match the version of Veeam Backup & Replication server. |

Tape Server

Tape Server

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Tape server connection state | State does not equal Accessible for more than 5 minutes. | Error | Automatic | Veeam Backup & Replication server lost connection to the tape server. |
| Tape server version is out-of-date | Component version mismatch. | Warning | Automatic | Veeam tape server version does not match the version of Veeam Backup & Replication server. |

Cloud Repository

Cloud Repository

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Cloud repository free space | Free space is below 10%. | Warning | Automatic | Cloud repository is low on available free space. |
| Free space is below 5%. | Error |
| Cloud repository lease expiration date | 14 days to lease expiration. | Warning | Automatic | Cloud repository lease time is about to expire. |
| 0 days to lease expiration. | Error |
| VM backups in cloud repository | Number of stored VMs is above the specified threshold. | Warning | Automatic | Number of VMs stored in the cloud repository is above the defined threshold. |

Cloud Gateway

Cloud Gateway

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Cloud gateway connection state | State does not equal Accessible for more than 5 minutes. | Error | Automatic | Veeam Backup & Replication server lost connection to the cloud gateway. |
| Cloud gateway version is out-of-date | Component version mismatch. | Warning | Automatic | Veeam cloud gateway version does not match the version of Veeam Backup & Replication server. |

Computer

Computer

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Computer with no backup | No computer backups were created for more than 24 hours. | Warning | Automatic | This computer has not been backed up within the configured RPO (Recovery Point Objective) period. |

Enterprise Application

Enterprise Application

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Application with no recent data backup sessions | No backup jobs protecting application database finished successfully or with warnings for more than 24 hours. | Warning | Automatic | One or several databases on an application server or application cluster are not protected with a backup job that finished successfully or with warnings within the configured RPO (Recovery Point Objective) period. |

Intelligent Diagnostics

List of intelligent diagnostics alarms depends on the set of installed signatures. For details, see [Veeam Intelligent Diagnostics](https://helpcenter.veeam.com/docs/one/monitor/intelligent_diagnostics.html?ver=110).


