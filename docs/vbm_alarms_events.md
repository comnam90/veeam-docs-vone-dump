---
title: "Veeam Backup for Microsoft 365 Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbm_alarms_events.html"
last_updated: "10/31/2025"
product_version: "13.0.1.6168"
---

# Veeam Backup for Microsoft 365 Alarms


This section describes predefined alarms for Veeam Backup for Microsoft 365 infrastructure components.

Veeam Backup for Microsoft 365 Server

|  |
| --- |
| Note: |
| For the Restore Activity (Veeam Backup for Microsoft 365) alarm, Veeam ONE only collects information about restores from Veeam Backup for Microsoft 365 versions 8 and above. Restore data from versions below 8 is not presented in this alarm. |

Veeam Backup for Microsoft 365 Server

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Backup copy job state (Veeam Backup for Microsoft 365) | State of a backup copy job equals Warning. | Warning | Automatic | Backup copy job reported either an error or a warning. |
| State of a backup copy job equals Failed. | Error |
| Backup job state (Veeam Backup for Microsoft 365) | State of a backup job equals Warning. | Warning | Automatic | Backup job reported either an error or a warning. |
| State of a backup job equals Failed. | Error |
| Job disabled (Veeam Backup for Microsoft 365) | Job is disabled for more than 12 hours. | Warning | Automatic | Job stays in the disabled state for a longer time than configured in the alarm threshold. |
| License exceeded for Veeam Backup for Microsoft 365 | Based on event | Warning | Automatic | Number of protected user accounts exceeds the license limit. |
| Based on event | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| License expiration date (Veeam Backup for Microsoft 365) | Based on event VeeamVbmServerLicenseExpiration. | Warning | Automatic | Veeam Backup for Microsoft 365 license expired. |
| Based on event VeeamVbmServerLicenseExpirationResolved. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Restore activity (Veeam Backup for Microsoft 365) | A restore operation of any type has been completed in the organization. | Information | Manual | A restore session has been performed on a Veeam Backup for Microsoft 365 server. |
| Organization with no backup | Microsoft 365 organization has no restore points created within the last 24 hours. | Warning | Automatic | Microsoft 365 organization was not backed up during the configured RPO period. |
| Unusual job duration (Veeam Backup for Microsoft 365) | Job duration is above 150% of average time interval. | Warning | Automatic | Job duration is above usual values among the set of job sessions. |
| Job duration is above 200% of average time interval. | Error |
| Veeam ONE server failed to connect to Microsoft 365 server | State does not equal Connected for more than 5 minutes. | Error | Automatic | Connection to Veeam Backup for Microsoft 365 server failed. |
| Veeam Backup for Microsoft 365 service state | Veeam Backup for Microsoft 365 service status does not equal Running for more than 5 minutes. | Error | Automatic | Veeam Backup for Microsoft 365 service is not running on the Veeam Backup for Microsoft 365 server. |

Backup Proxy

Backup Proxy

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Backup proxy connection failure (Veeam Backup for Microsoft 365) | Backup proxy status does not equal Online for more than 5 minutes. | Error | Automatic | Veeam Backup for Microsoft 365 server lost connection to the proxy server. |
| Backup proxy maintenance mode state (Veeam Backup for Microsoft 365) | Backup proxy maintenance mode is enabled. | Warning | Automatic | Backup proxy maintenance mode is enabled. |

Backup Repository

Backup Repository

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Backup repository free space (Veeam Backup for Microsoft 365) | Free space is below 5%. | Error | Automatic | Backup repository is low on free space. |
| Free space is below 10%. | Warning |
| Immutability change tracking (Veeam Backup for Microsoft 365) | Based on event VeeamImmutabilityIntervalDaysDecreased. | Warning | Manual | The configured immutability period has been changed on one or several Veeam Backup for Microsoft 365 repositories. |
| Based on event VeeamImmutabilityIntervalDaysIncreased. |
| Based on event VeeamImmutabilityIntervalDaysEnabled. |


