---
title: "Internal Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/internal_alarms_events.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Internal Alarms


The following table describes internal Veeam ONE alarms.

Internal Alarms

| Alarm Name | Event/Condition | Severity | Description |
| Audit log failure | Based on event VeeamAuditLogFailureEvent. | Error | Veeam ONE failed to add a new record to the audit log. |
| Based on event VeeamAuditLogFailureResolvedEvent. | Resolve |
| Audit log free space | Amount of free space is below 25%. | Warning | Size of the audit log is reaching the maximum allocated space limit. |
| Amount of free space is below 5%. | Error |
| Backup performance data collection failure | Based on event VeeamBpPerfCollectionFailedEvent. | Error | Veeam ONE failed to collect performance data from the specified backup server. |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Based on event VeeamBpPerfCollectionFailedResolvedEvent. | Resolve |
| Backup data collection failure | Based on event VeeamNoHostConnectionEvent. | Error | Veeam ONE failed to collect data from a Veeam Backup & Replication and Veeam Backup for Microsoft 365 server. |
| Based on event VeeamNoHostConnectionResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Disk cache error | Based on event VeeamDPCacheEvent. | Warning | Veeam ONE failed to write performance data to the disk cache folder. |
| Based on event VeeamDPCacheResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Events data collection failure | Based on event VeeamEventCollectionFailedEvent. | Error | Veeam ONE failed to collect events data from the objects specified. |
| Based on event VeeamEventCollectionFailedResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Guest services collection failure | Based on event VeeamCollectionServiceFailedEvent. | Error | Veeam ONE failed to collect guest services state information. |
| Based on event VeeamCollectionServiceFailedResolvedEvent. | Resolve |
| Guest processes collection failure | Based on event VeeamCollectionProcessFailedEvent. | Error | Veeam ONE failed to collect guest processes state information. |
| Based on event VeeamCollectionProcessFailedResolvedEvent. | Resolve |
| Hardware sensors collection failure | Based on event VeeamHardwareSensorsCollectionEvent. | Error | Veeam ONE failed to collect host hardware information. |
| Based on event VeeamHardwareSensorsCollectionResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Performance data collection failure | Based on event VeeamPerfCollectionFailedEvent. | Error | Veeam ONE failed to collect performance data from the objects specified. |
| Based on event VeeamPerfCollectionFailedResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Recon Scanner threat state | Status of threat detection equals Information. | Information | Recon Scanner raised the alert based on one or more suspicious behaviors. |
| Status of threat detection equals Warning. | Warning |
| Status of threat detection equals Error. | Error |
| Reporting data scheduling issue | Status of a report scheduling task equals Warning. | Warning | Veeam ONE failed to deliver a scheduled report, report folder or dashboard. |
| Status of a report scheduling task equals Failed. | Error |
| Status of a report folder scheduling task equals Warning. | Warning |
| Status of a report folder scheduling task equals Failed. | Error |
| Status of a dashboard scheduling task equals Warning. | Warning |
| Status of dashboard scheduling task equals Failed. | Error |
| SQL Server Express database size | Based on event VeeamSqlLowDbFreeSpaceEvent. | Warning | Veeam ONE database size is close to maximum database size supported by SQL Server Express Edition. |
| Based on event VeeamSqlLowDbFreeSpaceResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Staging data processing issue | Age of the oldest file that contains staging data equals 1 day. | Error | Age of the oldest file that contains staging data of Veeam ONE databases has reached the configured threshold. |
| Topology collection failure | Based on event VeeamInfCollectionFailedEvent. | Error | Veeam ONE failed to collect infrastructure topology. |
| Based on event VeeamInfCollectionFailedResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| VMware Cloud Director blocking tasks update failure | Based on event VeeamVcdBlockingTaskUpdateFailedEvent. | Error | Veeam ONE failed to update VMware Cloud Director blocking tasks list. |
| Based on event VeeamVcdBlockingTaskUpdateFailedResolvedEvent. | Resolve |
| VMware Cloud Director connection failure | Based on event VeeamNoVcdHostConnectionEvent. | Error | Veeam ONE failed to collect performance and configuration data from VMware Cloud Director. |
| Based on event VeeamNoVcdHostConnectionResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| VMware Cloud Director stranded items update failure | Based on event VeeamVcdStrandedItemUpdateFailedEvent. | Error | Veeam ONE failed to update VMware Cloud Director stranded items list. |
| Based on event VeeamVcdStrandedItemUpdateFailedResolvedEvent. | Resolve |
| Veeam Backup & Replication license compatibility | Based on event VeeamBackupServerLicenseCompatibility. | Error | License installed on the backup server is not compatible with the license installed on Veeam ONE server. |
| Based on event VeeamBackupServerLicenseCompatibilityResolved. | Resolve |
| Veeam Analytics service on the Veeam ONE server is not running | Based on event VeeamOneAgentServerNoConnectionEvent. | Error | Veeam Analytics service on the Veeam ONE server is not running. |
| Based on event VeeamOneAgentServerNoConnectionResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Veeam Analytics service on the remote server is not running | Based on event VeeamOneAgentClientNoConnectionEvent. | Error | Veeam Analytics service on the remote server is not running. |
| Based on event VeeamOneAgentClientNoConnectionResolvedEvent. | Resolve |
| Veeam intelligent diagnostics failure | Based on event VeeamIntelligenceDiagnosisFailedEvent. | Error | Veeam ONE failed to analyze Veeam Backup & Replication server logs. |
| Veeam ONE agent server connection failure | Based on event VeeamOneAgentServerNoConnectionEvent. | Error | Veeam ONE server failed to connect to Veeam ONE agent server. |
| Based on event VeeamOneAgentServerNoConnectionResolvedEvent. | Resolve |
| Veeam ONE agent client connection failure | Based on event VeeamOneAgentClientNoConnectionEvent. | Error | Veeam ONE server failed to connect to Veeam ONE agent client. |
| Based on event VeeamOneAgentClientNoConnectionResolvedEvent. | Resolve |
| Veeam ONE Caching service state | Veeam ONE caching service failed. | Error | Veeam ONE Caching service not started or is not working properly. |
| Veeam ONE Caching service database state | Based on event VeeamCachingServiceDatabaseIsDownEvent | Error | Veeam ONE Caching service database not started or is not working properly. |
| Based on event VeeamCachingServiceDatabaseIsDownResolvedEvent | Resolve | Veeam ONE Caching service database error resolved. |
| Based on event VeeamMonitorServiceStartedEvent | Resolve | Veeam ONE Monitor service database service started. |
| Veeam ONE database cleanup task status | Database object removal queue constantly grew for defined time period (default 1 day). | Error | Veeam ONE server processing speed is slower than the deletion of object information. |
| Veeam ONE email notification delivery failure | Based on event VeeamEmailNotificationFailed. | Error | Veeam ONE server failed to deliver an email notification. |
| Based on event VeeamEmailNotificationResolved. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Veeam ONE license expiration date | Based on event VeeamLicenseExpirationWarningEvent. | Warning | Veeam ONE license is going to expire soon. |
| Based on event VeeamLicenseExpirationErrorEvent. | Error |
| Based on event VeeamLicenseChangedEvent. | Resolve |
| Based on event VeeamLicenseExpirationResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Veeam ONE license update failure | Based on event VeeamLicenseUpdateErrorEvent. | Warning | License update failure can take place for a number of reasons such as connection failure, invalid identifier, expired contract, and so on. In case of a connection problem and licensing server key generation error, Veeam ONE will retry to update the license key. |
| Based on event VeeamLicenseUpdateResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Veeam ONE license exceeded | Based on event VeeamVMsExceedErrorEvent. | Error | Veeam ONE license limit has been exceeded. |
| Based on event VeeamVMsExceedWarningEvent. | Warning |
| Based on event VeeamSocketExceedEvent. | Error |
| Based on event VeeamBpExceedErrorEvent. | Error |
| Based on event VeeamBpExceedWarningEvent. | Warning |
| Based on event VeeamLicenseGraceOverEvent. | Error |
| Based on event VeeamVMsExceedResolvedEvent. | Resolve |
| Based on event VeeamSocketExceedResolvedEvent. | Resolve |
| Based on event VeeamLicenseChangedEvent. | Resolve |
| Based on event VeeamVbmExceedWarningEvent. | Warning |
| Based on event VeeamVbmExceedResolvedEvent. | Resolve |
| Object properties data collection failure | Job state equals Failed. | Error | Veeam ONE Object properties data collection job did not finish successfully. |
| Job state equals Warning. | Warning |
| Veeam ONE Reporting service state | Veeam ONE Reporting service is not running. | Error | Veeam ONE Reporting service has failed. |
| Veeam ONE Server Load | Veeam ONE Server CPU Usage is above 90% or Veeam ONE Server Memory Usage is above 95%. | Error | Veeam ONE Server load is too high. |
| Veeam ONE Server CPU Usage is above 75% or Veeam ONE Server Memory Usage is above 85%. | Warning |
| Veeam ONE support expiration date | Based on event VeeamLicenseSupportExpirationWarningEvent. | Warning | Veeam ONE support period is going to expire soon. |
| Based on event VeeamLicenseSupportExpirationErrorEvent. | Error |
| Based on event VeeamLicenseChangedEvent. | Resolve |
| Based on event VeeamLicenseSupportExpirationResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| Virtual Server connection failure | Based on event VeeamNoHostConnectionEvent. | Error | Connection to virtual server has failed. |
| Based on event VeeamNoHostConnectionResolvedEvent. | Resolve |
| Based on event VeeamMonitorServicesStartedEvent. | Resolve |
| ServiceNow instance connection state | Based on event VeeamServiceNowNoConnectionEvent | Error | Connection to ServiceNow instance has failed. |
| Based on event VeeamServiceNowNoConnectionResolvedEvent | Resolve |
| Based on event VeeamMonitorServicesStartedEvent | Resolve |
| Syslog server connection state | Based on event VeeamSyslogServerFailureEvent | Error | The Syslog server is unavailable. |
| Based on event VeeamSyslogServerFailureResolvedEvent | Resolve |
| Based on event VeeamMonitorServicesStartedEvent | Resolve |

Page updated 2026-07-30

