---
title: "VMware vSphere Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vsphere_alarms_events.html"
last_updated: "10/31/2025"
product_version: "13.0.1.6168"
---

# VMware vSphere Alarms


This section describes predefined alarms for VMware vSphere infrastructure components.

vCenter Server

vCenter Server

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Bad vCenter Server username logon attempt | Based on event | Error | Manual | This event records a failed user logon. The combination of username, password, and permissions is the mechanism by which vCenter Server authenticate a user for access and authorize the user to perform activities. |
| Insufficient user access permissions | Based on event | Error | Manual | This event records a failed user logon due to insufficient access permission. |
| Invalid license edition | Based on event InvalidEditionEvent. | Error | Manual | This event records if the license edition is set to an invalid value. |
| License expired | Based on event LicenseExpiredEvent. | Error | Manual | This event records the expiration of a license. |
| License file restricted | Based on event LicenseRestrictedEvent. | Error | Manual | This event records if the required licenses could not be reserved because of a restriction in the option file. |
| License is not compliant | Based on event LicenseNonComplianceEvent. | Error | Manual | This event records that the inventory is not license compliant. |
| Maximum host connections reached | Based on event HostInventoryFullEvent. | Error | Manual | This event records if the inventory of hosts has reached capacity. |
| No license reservation | Based on event NoLicenseEvent. | Error | Manual | These are events reported by License Manager. A NoLicenseEvent is reported if the required licenses could not be reserved. Each feature that is not fully licensed is reported. |
| Non VI workload detected | Based on event NonVIWorkloadDetectedOnDatastoreEvent. | Error | Manual | A potential misconfiguration or I/O performance issue caused by a non-ESX workload has been detected. This alarm is triggered when Storage I/O Control (SIOC) detects that a workload that is not managed by SIOC is contributing to I/O congestion on a datastore that is managed by SIOC. |
| vCenter Server agent uninstall failure | Based on event VcAgentUninstallFailedEvent. | Error | Manual | This event records when the vCenter Server agent on a host failed to uninstall. |
| vCenter Server agent upgrade failure | Based on event VcAgentUpgradeFailedEvent. | Error | Manual | This event records when the vCenter Server agent on a host failed to upgrade. |
| vCenter Server license expired | Based on event ServerLicenseExpiredEvent. | Error | Manual | This event records an expired vCenter Server license. |

Cluster

Cluster

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Admission control disabled | Based on event DasAdmissionControlDisabledEvent. | Information | Automatic | This event records when admission control checks have been disabled in a HA cluster. |
| Admission control enabled | Based on event DasAdmissionControlEnabledEvent. | Information | Automatic | This event records when admission control checks have been enabled in a HA cluster. |
| All hosts in cluster isolated | Based on event DasClusterIsolatedEvent. | Error | Manual | This event records that all hosts have been isolated from the network in a HA cluster. |
| DRS invocation failure | Based on event DrsInvocationFailedEvent. | Error | Manual | This event records DRS invocation failure. DRS invocation not completed. |
| HA disabled for cluster | Based on event DasDisabledEvent. | Information | Automatic | This event records when a cluster has been disabled for HA. |
| HA enabled for cluster | Based on event DasEnabledEvent. | Information | Automatic | This event records when a cluster has been enabled for HA. |
| Host cluster capacity overcommitted | Based on event ClusterOvercommittedEvent. | Error | Manual | This event records when a cluster's host capacity cannot satisfy resource configuration constraints. |
| vSphere cluster warning | Based on event com.vmware.vc.HA.ClusterContainsIncompatibleHosts. | Warning | Manual | One of the hosts in an HA cluster has been isolated. |
| Based on event com.vmware.vc.HA.DasFailoverHostIsolatedEvent. |
| Based on event com.vmware.vc.HA.DasFailoverHostPartitionedEvent. |
| Based on event com.vmware.vc.HA.DasFailoverHostUnreachableEvent. |
| Based on event com.vmware.vc.HA.DasHostIsolatedEvent. |

Host

Host

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Bad Host username logon attempt | Based on event BadUsernameSessionEvent. | Warning | Manual | This event records a failed user logon. The combination of username, password, and permissions is the mechanism by which hosts authenticate a user for access and authorize the user to perform activities. |
| Connection to iSCSI storage target failure | Based on event esx.problem.storage.iscsi.discovery.connect.error. | Error | Manual | The iSCSI initiator is unable to establish a connection to the target. |
| Based on event esx.problem.storage.iscsi.discovery.login.error. |
| Based on event esx.problem.storage.iscsi.target.connect.error. |
| Based on event esx.problem.storage.iscsi.target.login.error. |
| DPM failed to bring host out of standby mode | Based on event DrsExitStandbyModeFailedEvent. | Error | Automatic | This event records that Distributed Power Management tried to bring a host out of standby mode, but failed.  Standby Mode powers off a host and allows it to be powered back on again through the Wake-on-LAN protocol. It can be triggered either manually or automatically by vCenter Server. |
| Based on event DrsExitedStandbyMode. | Resolve |
| Based on event ExitedStandbyMode. | Resolve |
| DRS host standby mode entrance | Based on event DrsEnteredStandbyModeEvent. | Information | Automatic | This event records that the host has successfully entered standby mode initiated by Distributed Power Management. A host in this mode has no running virtual machines and no provisioning operations are occurring. |
| DRS host standby mode exit | Based on event DrsExitedStandbyModeEvent. | Information | Automatic | This event records that Distributed Power Management brings this host out from standby mode. |
| DRS synchronization failure | Based on event DrsResourceConfigureFailedEvent. | Error | Manual | This event records when resource configuration specification synchronization fails on a host. |
| DVS host configuration out of sync | Based on event OutOfSyncDvsHost. | Warning | Manual | The list of hosts that have the DVS configuration on the host diverged from that of the vCenter Server. |
| ESXi host network uplink failure | Based on event esx.problem.net.lacp.uplink.fail.duplex. | Error | Manual | Link Aggregation Control Protocol (LACP) is included in IEEE specification as a method to control the bundling of several physical ports together to form a single logical channel. LACP allows a network device to negotiate an automatic bundling of links by sending LACP packets to the peer (directly connected device that also implements LACP). |
| Based on event esx.problem.net.lacp.uplink.fail.speed. |
| Based on event esx.problem.net.lacp.uplink.inactive. |
| ESXi host CPU hardware error | Based on event esx.problem.cpu.amd.mce.dram.disabled. | Error | Manual | ESXi host has experienced a CPU hardware error. |
| Based on event esx.problem.cpu.intel.ioapic.listing.error. |
| Based on event esx.problem.cpu.mce.invalid. |
| Based on event esx.problem.cpu.smp.ht.invalid. |
| Based on event esx.problem.cpu.smp.ht.numpcpus.max. |
| ESXi host network error | Based on event esx.problem.dhclient.lease.none. | Error | Manual | DHCP client lease issue has been detected. |
| ESXi host network uplink problems | Based on event esx.problem.net.lacp.uplink.blocked. | Warning | Manual | Link Aggregation Control Protocol (LACP) is included in IEEE specification as a method to control the bundling of several physical ports together to form a single logical channel. LACP allows a network device to negotiate an automatic bundling of links by sending LACP packets to the peer (directly connected device that also implements LACP). |
| Based on event esx.problem.net.lacp.uplink.disconnected. |
| ESXi host network warning | Based on event esx.problem.dhclient.lease.offered.error. | Warning | Manual | DHCP client lease issue has been detected. |
| Based on event esx.problem.dhclient.lease.persistent.none. |
| ESXi host storage error | Based on event esx.problem.scsi.device.state.permanentloss.withreservationheld. | Error | Manual | Storage device becomes permanently lost while SCSI reservation is held by ESXi. |
| ESXi host storage failure | Based on event esx.problem.visorfs.failure. | Error | Manual | An operation on the root file system has failed. |
| ESXi host storage warning | Based on event esx.problem.visorfs.inodetable.full. | Warning | Manual | One of the host's ramdisks reached the limit for the number of files it can contain. |
| Based on event esx.problem.visorfs.ramdisk.full. | Warning |
| Host available memory | Average memory usage is for 15 minutes is above 80%. | Warning | Automatic | This host is low on available memory. |
| Average memory usage is for 15 minutes is above 90%. | Error |
| Host connection failure | Host state equals Disconnected for 5 minutes and more. | Warning | Automatic | This alarm monitors the VMware vCenter Server API for events indicating that a host is disconnected. |
| Host state equals Not responding for 5 minutes and more. |
| Host connectivity failure | Based on event vprob.net.connectivity.lost. | Error | Automatic | This event indicates that one or more portgroups in the host have lost connectivity to the network, resulting in unavailability of all physical connections to the network from this switch. |
| Based on event esx.problem.net.connectivity.lost. |
| Based on event esx.clear.net.connectivity.restored. | Resolve |
| Host CPU ready | Average CPU Ready for 15 minutes is above 15%. | Warning | Automatic | This Host has exceeded the threshold for CPU Ready Percent. |
| Average CPU Ready for 15 minutes is above 25%. | Error |
| Host CPU usage | Average CPU usage for 15 minutes is above 75%. | Warning | Automatic | This host has exceeded the threshold for CPU usage. |
| Average CPU usage for 15 minutes is above 95%. | Error |
| Host disk bus resets | Average datastore bus resets for 15 minutes is above 2. | Warning | Automatic | This host disk (vmhba) has logged one or more SCSI bus resets. |
| Average datastore bus resets for 15 minutes is above 4. | Error |
| Host disk SCSI aborts | Average datastore command aborts for 15 minutes is above 2. | Warning | Automatic | This host disk (vmhba) has logged one or more SCSI aborts. |
| Average datastore command aborts for 15 minutes is above 4. | Error |
| Host failed to exit standby mode | Based on event ExitStandbyModeFailedEvent. | Error | Automatic | This event records that the host failed to exit standby mode.  Standby Mode powers off a host and allows it to be powered back on again through the Wake-on-LAN protocol. It can be triggered either manually or automatically by vCenter Server. |
| Based on event ExitedStandbyMode. | Resolve |
| Host HA agent failure | Based on event com.vmware.vc.HA.HostAgentErrorEvent. | Error | Manual | Usually, such triggers indicate that a host has actually failed, but failure reports can sometimes be incorrect. A failed host reduces the available capacity in the cluster and, in the case of an incorrect report, prevents vSphere HA from protecting the virtual machines running on the host. |
| Host HA disabled | Based on event HostDasDisabledEvent. | Information | Automatic | This event records when HA has been disabled on a host. |
| Host HA enabled | Based on event HostDasEnabledEvent. | Information | Automatic | This event records when the HA (high-availability) agent has been enabled on a host. |
| Host hardware status | Hardware sensor equals Warning. | Warning | Automatic | One of the hosts' hardware sensors has changed its status. |
| Hardware sensor equals Alert. | Error |
| Hardware sensor equals Unknown. | Warning |
| Host IP inconsistent | Based on event HostIpInconsistentEvent. | Warning | Manual | This event records that the IP address resolution returned different addresses on the host. |
| Host IP to short name failed | Based on event HostIpToShortNameFailedEvent. | Warning | Manual | This event records that the host's IP address could not be resolved to a short name. |
| Host Isolation IP not available | Based on event HostIsolationIpPingFailedEvent. | Warning | Manual | This event records that the isolation address could not be pinged. The default isolation address is the service console's default gateway. |
| Host license expired | Based on event HostLicenseExpiredEvent. | Error | Manual | This event records an expired host license. |
| Host memory pressure | Average memory pressure for 15 minutes is above 150%. | Warning | Automatic | This host has exceeded the threshold for memory pressure. |
| Average memory pressure for 15 minutes is above 250%. | Error |
| Host NIC link status | Host NIC link status equals Down. | Error | Automatic | Physical NIC linkstate is down. |
| Host not compliant | Based on event HostNonCompliantEvent. | Warning | Manual | This event records that host went out of compliance. |
| Host operation cancelled | Based on event CanceledHostOperationEvent. | Information | Automatic | An operation performed on the host was canceled. |
| Host operation timed out | Based on event TimedOutHostOperationEvent. | Warning | Manual | This event indicates that an operation performed on the host timed out. |
| Host primary agent not in short name | Based on event HostPrimaryAgentNotShortNameEvent. | Warning | Manual | This event records that the primary agent specified is not a short name. |
| Host reconnection failed | Based on event HostConnectedEvent. | Resolve | Automatic | This event records a failed attempt to re-establish a host connection. |
| Based on event HostReconnectionFailedEvent. | Error |
| Host redundancy failure | Based on event vprob.net.redundancy.lost. | Warning | Automatic | The event indicates that one or more portgroups in the host has lost a redundant uplink to the physical network. Portgroups are still connected. However this may be the last redundant uplink. Check the event description and context to confirm the status. |
| Based on event vprob.net.redundancy.degraded. |
| Based on event esx.problem.net.redundancy.lost. |
| Based on event esx.problem.net.redundancy.degraded. |
| Based on event esx.clear.net.redundancy.restored. | Resolve |
| Host short name inconsistent | Based on event HostShortNameInconsistentEvent. | Warning | Manual | This event records that host name resolution returned different names on the host. |
| Host short name IP resolve failed | Based on event HostShortNameToIpFailedEvent. | Warning | Manual | This event records that the host's short name could not be resolved to an IP address. |
| Host swap memory | Average memory swap used for 15 minutes is above 64 MB. | Warning | Automatic | This host is swapping too much memory. |
| Average memory swap used for 15 minutes is above 128 MB. | Error |
| Host synchronization failed | Based on event HostSyncFailedEvent. | Warning | Manual | This event records a failure to sync up with the vCenter Server agent on the host. |
| Host upgrade connection failure | Based on event HostUpgradeFailedEvent. | Error | Manual | This event records a failure to connect to a host due to an installation or upgrade issue. |
| Incorrect host information | Based on event IncorrectHostInformationEvent. | Warning | Manual | This event records if the host did not provide the information needed to acquire the correct set of licenses. |
| iSCSI target storage connection failure | Based on event esx.problem.storage.iscsi.target.connected.error. | Error | Manual | The iSCSI initiator is unable to establish a connection to the target. |
| iSCSI targets are permanently removed from ESXi | Based on event esx.problem.storage.iscsi.target.permanently.lost. | Error | Manual | The esx.problem.storage.iscsi.target.permanently.removed message is received when an iSCSI target is no longer presented to ESXi. |
| Isolation addresses is missing | Based on event com.vmware.vc.HA.HostHasNoIsolationAddrsDefined. | Warning | Manual | ESXi host is missing isolation addresses for isolation detection. |
| Network rollback detected | Based on event NetworkRollbackEvent. | Error | Manual | In vSphere 5.1, rollback is enabled by default. However, you can enable or disable rollbacks at the vCenter Server level. Several networking events can trigger a rollback. The events are grouped into these categories:   * Host networking rollbacks (virtual switches or network system) * Distributed switch rollbacks |
| No host network for HA available | Based on event HostNoAvailableNetworksEvent. | Warning | Manual | This event records the fact that a host does not have any available networks for HA communication. |
| Non VI workload detected on host | Based on event EsxProblemIormNonViWorkload. | Error | Manual | A potential misconfiguration or I/O performance issue caused by a non-ESX workload has been detected. This alarm is triggered when Storage I/O Control (SIOC) detects that a workload that is not managed by SIOC is contributing to I/O congestion on a datastore that is managed by SIOC. |
| SCSI unsupported plugin warning | Based on event esx.problem.scsi.unsupported.plugin.type. | Warning | Manual | An invalid storage module attempted to configure a SCSI device. |
| Storage connection failure | Based on event vprob.storage.connectivity.lost. | Error | Automatic | The event indicates a loss in connectivity to the specified storage device. The path indicated is the last path that went down. |
| Based on event esx.problem.storage.connectivity.lost. |
| Based on event esx.clear.storage.connectivity.restored. | Resolve |
| Storage connection redundancy failure | Based on event vprob.storage.redundancy.lost. | Warning | Automatic | A host has lost a path to access the specified storage and the path to storage is either degraded, or no longer redundant. Check the event description and context to confirm the status. |
| Based on event vprob.storage.redundancy.degraded. |
| Based on event esx.problem.storage.redundancy.degraded. |
| Based on event esx.problem.storage.redundancy.lost. |
| Based on event esx.clear.storage.redundancy.restored. | Resolve |
| Teaming mismatch error | Based on event TeamingMisMatchEvent. | Error | Manual | The teaming configuration of the uplink ports in the DVS does not match physical switch configuration. |
| Uplink port MTU error | Based on event UplinkPortMtuNotSupportEvent. | Error | Manual | MTU health check status of an uplink port is changed. |
| Uplink port VLAN error | Based on event UplinkPortVlanUntrunkedEvent. | Error | Manual | Vlans health check status of an uplink port is changed. |
| vCenter Server lost connection to host | Based on event HostConnectionLostEvent. | Error | Automatic | vCenter Server has lost connection to this host. |
| Based on event HostCnxFailed. |
| Based on event HostConnectedEvent. | Resolve |
| vMotion license expired | Based on event VMotionLicenseExpiredEvent. | Error | Manual | This event records an expired vMotion license. |
| vSphere Distributed Switch MTU mismatch | Based on event MtuMismatchEvent. | Error | Manual | A larger MTU (maximum transmission unit) bring greater efficiency because each packet carries more user data while protocol overheads; the resulting higher efficiency means a slight improvement in bulk protocol throughput. A larger MTU also means processing of fewer packets for the same amount of data. However, this gain is not without some downside. Large packets can occupy a slow link for some time, causing greater delays to following packets and increasing lag and minimum latency. |

Virtual Machine

Virtual Machine

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Customization unknown failure | Based on event CustomizationUnknownFailure. | Warning | Manual | The customization sequence failed unexpectedly in the guest. |
| Fault Tolerance VM terminated | Based on event VmFaultToleranceVmTerminatedEvent. | Warning | Manual | This event records a secondary or primary VM is terminated. |
| FT VM Failover | Based on event VmPrimaryFailoverEvent. | Error | Manual | This event records a fault tolerance failover. |
| Guest customization failure | Based on event CustomizationFailed. | Warning | Manual | The customization sequence in the guest failed. Cannot complete customization of VM. |
| Guest disk space | Guest disk free space space is below 10%. | Warning | Automatic | Guest OS volume is low on available guest disk space. |
| Guest disk free space space is below 5%. | Error |
| HA agent update failed | Based on event VmDasUpdateErrorEvent. | Error | Manual | The event records an error occurred when updating the HA agents with the current state of the VM. |
| Heartbeat is missing for VM | Heartbeat not detected for 15 minutes. | Error | Automatic | The heartbeat is the communication to the VMware tools heartbeat running inside the VM.  Heartbeat can only be monitored when the VMware tools are installed in a VM. The heartbeat is what vCenter Server uses to determine the general health and availability of a running VM. |
| High balloon memory utilization | Average memory balloon percent for 15 minutes is above 10%. | Warning | Automatic | There is high utilization of the VMware Tools memory controller, also known as the 'balloon driver', within this VM. |
| Average memory balloon percent for 15 minutes is above 50%. | Error |
| High memory usage | Average memory usage for 15 minutes is above 90%. | Warning | Automatic | There is high utilization of memory within this Virtual Machine. The memory active metric is the current percentage of memory active vs. memory maximum for this VM. |
| Average memory usage for 15 minutes is above 95%. | Error |
| Latest snapshot age | VM snapshot age is 48 hour or more. | Warning | Automatic | The age of the latest snapshot for this VM has exceeded the configured threshold. |
| Latest snapshot size | VM snapshot size is above 10%. | Warning | Automatic | The size of the latest snapshot file for this VM has exceeded the configured threshold. |
| VM snapshot size is above 20%. | Error |
| Linux customization identity failure | Based on event CustomizationLinuxIdentityFailed. | Warning | Manual | Failed to set Linux identity. |
| Potential infrastructure malware activity | Potential malware activity is infected | Error | Automatic | Veeam Backup & Replication server has detected potential malware activity. |
| Potential malware activity is suspicious | Warning |
| Network customization setup failure | Based on event CustomizationNetworkSetupFailed. | Warning | Manual | Network setup failed in the guest during customization. |
| No compatible host for Secondary VM | Based on event VmNoCompatibleHostForSecondaryEvent. | Warning | Manual | This event records that no compatible host was found to place a secondary VM. A default alarm will be triggered upon this event, which by default, triggers a SNMP trap. |
| No host for a virtual machine available | Based on event VmOrphanedEvent. | Warning | Manual | This event records a VM for which no host is responsible. |
| No maintenance mode DRS recommendation for VM | Based on event NoMaintenanceModeDrsRecommendationForVM. | Warning | Manual | This event records that DRS did not recommend a migration for a powered on VM, even though its host is going into maintenance mode. |
| No network access for VM migration | Based on event VmNoNetworkAccessEvent. | Warning | Manual | This event records a migration failure when the destination host is not on the same network as the source host. |
| Not enough resources for failover | Based on event NotEnoughResourcesToStartVmEvent. | Warning | Manual | This event records when the HA does not find sufficient resources to failover a VM. |
| Orphaned VM backup snapshot | Orphaned VM backup snapshot age is 60 minutes or more. | Error | Automatic | This VM is running on the snapshot left by backup or replication job. |
| Possible ransomware activity | Average CPU Usage is above 70%  and  Datastore Write Rate is above 40 MB/s  or Network Transmit Rate is above 40 MB/s for 5 minutes. | Warning | Automatic | Veeam ONE detected suspicious activity on this VM. |
| Average CPU Usage is above 80%  and  Datastore Write Rate is above 60 MB/s  or Network Transmit Rate is above 60 MB/s for 5 minutes. | Error |
| Secondary VM config update failed | Based on event VmFailedUpdatingSecondaryConfig. | Warning | Manual | This event is recorded after a failover of the new primary VM failed to update the config of the secondary VM. |
| Secondary VM failed to start | Based on event VmFailedStartingSecondaryEvent. | Warning | Manual | The Secondary VM cannot be powered on as there are no compatible hosts that can accommodate it. |
| Secondary VM start timeout | Based on event VmTimedoutStartingSecondaryEvent. | Warning | Manual | This event records timeout when starting a secondary VM. |
| Sysprep customization failure | Based on event CustomizationSysprepFailed. | Warning | Manual | Sysprep failed to run in the guest during customization. This can be caused by the fact that the wrong sysprep was used for the guest or errors in the sysprep file. |
| Too many snapshots on the VM | Number of VM snapshots is 3 or more. | Warning | Automatic | An excessive number of snapshots in a chain has been detected on the VM which may lead to decreased virtual machine and host performance. |
| Number of VM snapshots is 5 or more. | Error |
| Virtual disk creation failed | Based on event VmDiskFailedEvent. | Error | Manual | This event records a failure to create a virtual disk in a VM. |
| VM clone operation failure | Based on event VmCloneFailedEvent. | Error | Manual | This event records a failure to clone a VM. |
| VM configuration file missing | Based on event VmConfigMissingEvent. | Warning | Manual | This event records if the configuration file (VMX file) for a VM cannot be found. |
| VM connection failure | Based on event VmDisconnectedEvent. | Error | Automatic | This VM is 'Disconnected' in vCenter Server. |
| Based on event VmConnectedEvent. | Resolve |
| VM consolidation needed status | Based on event com.vmware.vc.VmDiskConsolidationNeeded. | Error | Automatic | When initiating Delete or DeleteAll operations on snapshots, the snapshot details are deleted from Snapshot Manager, then the snapshot files are consolidated and merged to another snapshot file or to the virtual machine parent disk. If the consolidation fails, there were no snapshots shown in the Snapshot Manager, but the snapshot files were still being used on the datastore. This can cause the datastore to run out of space. |
| Based on event com.vmware.vc.VmDiskConsolidationNoLongerNeeded. | Resolve |
| Based on event com.vmware.vc.VmDiskConsolidatedEvent. | Resolve |
| VM CPU ready | Average CPU ready all cores metric for 15 minutes is above 10%. | Warning | Automatic | This VM has exceeded the threshold for CPU Ready Percent. |
| Average CPU ready all cores metric for 15 minutes is above 20%. | Error |
| VM CPU usage | Average CPU usage for 15 minutes is above 75%. | Warning | Automatic | This VM has exceeded the threshold for CPU usage. |
| Average CPU usage for 15 minutes is above 90%. | Error |
| VM disk consolidation failure | Based on event com.vmware.vc.VmDiskFailedToConsolidateEvent. | Error | Automatic | There is an issue with the disk for this virtual machine. |
| Based on event com.vmware.vc.VmDiskConsolidatedEvent. | Resolve |
| VM disk SCSI connection failures | Average number of datastore command aborts for 15 minutes is above 2. | Warning | Automatic | This VMGuest disk connection (LUN) has logged one or more SCSI aborts. |
| Average number of datastore command aborts for 15 minutes is above 6. | Error |
| VM disk SCSI connection resets | Average number of datastore bus resets for 15 minutes is above 2. | Warning | Automatic | This VMGuest disk connection (LUN) has logged one or more SCSI bus resets. |
| Average number of datastore bus resets for 15 minutes is above 6. | Error |
| VM generic error | Based on event VmMessageErrorEvent. | Error | Manual | This is a generic event for error messages from a VM that do not fit into any other specific vCenter Server event. |
| VM generic warning | Based on event VmMessageWarningEvent. | Warning | Manual | This is a generic event for warning messages from a VM that did not fit into any other specific vCenter Server event. |
| VM guest reboot | Based on event VmGuestRebootEvent. | Information | Automatic | This is a VM guest reboot request event. |
| VM guest shutdown | Based on event VmGuestShutdownEvent. | Information | Automatic | This is a VM guest shutdown request event. |
| VM HA error | Based on event com.vmware.vc.HA.FailedRestartAfterIsolationEvent. | Error | Manual | vSphere HA has failed to restart after a host isolation. |
| VM HA reset | Based on event VmDasBeingResetEvent. | Warning | Manual | This event records when a VM is reset by HA VM Health Monitoring on hosts that do not support the create screenshot APIi or if the create screenshot API fails. |
| VM HA reset failure | Based on event VmDasResetFailedEvent. | Warning | Manual | This event records when HA VM health monitoring fails to reset a VM after failure. |
| VM memory swap usage | Average memory swapped for 15 minutes is above 64 MB. | Warning | Automatic | This VM has exceeded the threshold for memory swapping to disk within the host. |
| Average memory swapped for 15 minutes is above 128 MB. | Error |
| VM power status | State not equals Running for 5 minutes or more. | Error | Automatic | The power state of a VM indicates whether the VM is active and functional. |
| VM resetting | Based on event VmResettingEvent. | Information | Automatic | This event records a VM resetting. |
| VM restart on alternate host | Based on event VmRestartedOnAlternateHostEvent. | Information | Automatic | This event records that the VM was restarted on a host, since its original host had failed. |
| VM Screenshot HA reset | Based on event VmDasBeingResetWithScreenshotEvent. | Warning | Manual | This event records when a VM is reset by HA VM health monitoring on hosts that support the create screenshot API. |
| VM total disk latency | Average datastore highest latency for 15 minutes is above 50 milliseconds. | Warning | Automatic | Highest latency value across all disks used by the VM. |
| Average datastore highest latency for 15 minutes is above 75 milliseconds. | Error |
| VM with no backups | No backup restore points for the past 24 hours. | Warning | Automatic | This VM has not been backed up within the defined RPO (Recovery Point Objective) interval. |
| VM with no replica | No replica restore points for the past 24 hours. | Warning | Automatic | This VM has not been replicated within the defined RPO (Recovery Point Objective) interval. |
| VM WWN conflict | Based on event VmWwnConflictEvent. | Error | Manual | This event records a conflict of VM WWNs (World Wide Name). |
| VMware VM tools state | VMware VM tools state changes equals Unknown. | Warning | Automatic | There is a problem with VMware Tools in this Virtual Machine. |
| VMware VM tools state changes equals Out-of-date. | Warning |
| VMware VM tools state changes equals Not installed. | Error |
| VMware VM tools state changes equals Not running. | Error |

Datastore

Datastore

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Datastore free space | Free space is below 10%. | Warning | Automatic | Datastore is low on available free space. |
| Free space is below 5%. | Error |
| Datastore is inaccessible | State not equals Accessible for 5 minutes or more. | Error | Automatic | The event indicates a loss in connectivity to the specified storage device. The path indicated is the last path that went down. |
| Datastore over-allocation | Datastore provisioning rate is above 400%. | Warning | Automatic | Datastore is over-allocated. |
| Datastore provisioning rate is above 600%. | Error |
| Datastore read latency | Maximum datastore read latency for 15 minutes is above 100 milliseconds. | Warning | Automatic | Datastore latency has exceeded the threshold of total read latency. |
| Maximum datastore read latency for 15 minutes is above 250 milliseconds. | Error |
| Datastore write latency | Maximum datastore write latency for 15 minutes is above 100 milliseconds. | Warning | Automatic | Datastore latency has exceeded the threshold of total write latency. |
| Maximum datastore write latency for 15 minutes is above 250 milliseconds. | Error |
| Locker misconfiguration | Based on event LockerMisconfiguredEvent. | Warning | Manual | Locker has not been configured properly. Datastore which is configured to back the locker does not exist. |

Any Object

Any Object

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Duplicate IP address detected | Based on event DuplicateIpDetectedEvent. | Warning | Manual | This event records that a duplicate IP address has been observed, with conflict between VM, and the vMotion or IP storage interface configured on the host. |
| Host cluster destroyed | Based on event ClusterDestroyedEvent. | Information | Automatic | This event records when a cluster is destroyed. |
| Host failure detected | Based on event DasHostFailedEvent. | Error | Manual | This event records when a host failure has been detected by HA. |
| Host isolation in HA cluster | Based on event DasHostIsolatedEvent. | Warning | Manual | This event records that a host has been isolated from the network in a HA cluster. Since an isolated host cannot be distinguished from a failed host except by the isolated host itself, this event is logged when the isolated host regains network connectivity. |
| No host redundant management network available | Based on event HostNoRedundantManagementNetworkEvent. | Warning | Manual | This event records the fact that a host does not have a redundant management network. It is recommended that host management networks be configured with redundancy. |
| Primary host connection re-established | Based on event DasAgentFoundEvent. | Information | Automatic | This event records that vCenter Server has re-established contact with a primary host in this HA cluster. |
| Primary host unavailable | Based on event DasAgentUnavailableEvent. | Error | Automatic | This event records that vCenter Server cannot contact to any primary host in this HA cluster. vCenter Server has lost contact with all primary nodes with a connected state. Attempts to configure HA on a host in this cluster will fail until a DasAgentFoundEvent is logged or unless this is the first node to be configured. For example, if all the other hosts are disconnected first. |
| Based on event DasAgentFoundEvent. | Resolve |
| Resource pool configuration conflict | Based on event ResourceViolatedEvent. | Error | Manual | This event records when a conflict with a resource pool's resource configuration is detected. |
| Storage ATS support failure | Based on event esx.problem.vmfs.ats.support.lost. | Error | Manual | In a shared storage environment, when multiple hosts access the same VMFS datastore, specific locking mechanisms are used. These locking mechanism prevent multiple hosts from concurrently writing to the metadata and ensure that no data corruption occurs. VMFS supports SCSI reservations and atomic test and set (ATS) locking. For storage devices that support hardware acceleration, VMFS uses the ATS algorithm, also called hardware assisted locking. In contrast with SCSI reservations, ATS supports discrete locking per disk sector. |
| Task timeout reached | Based on event TaskTimeoutEvent. | Warning | Manual | This event records when a task exceeds defined timeout in vCenter Server. |
| Template deployment failure | Based on event VmDeployFailedEvent. | Error | Manual | This event records a failure to deploy a VM from a template. |
| vCenter storage availability error | Based on event vprob.vmfs.error.volume.is.locked. | Error | Manual | The alarm indicates that a VMFS volume on the ESXi host is locked due to an I/O error. |
| Based on event esx.problem.vmfs.error.volume.is.locked. | Error |
| Based on event vprob.vmfs.extent.offline. | Warning |
| Based on event esx.problem.vmfs.extent.offline. | Warning |
| VM instance UUID conflict | Based on event VmInstanceUuidConflictEvent. | Warning | Automatic | This event records a conflict of VM instance UUIDs. |
| Based on event VmInstanceUuidChangedEvent. | Resolve |
| VM MAC address conflict | Based on event VmMacConflictEvent. | Error | Automatic | This event records a MAC address conflict for a VM. |
| Based on event VmStaticMacConflictEvent. |
| Based on event VmMacChangedEvent. | Resolve |
| vSphere cluster HA error | Based on event com.vmware.vc.HA.HostDasErrorEvent. | Error | Manual | There is an issue with VMware high-availability configuration for this host. |
| vSphere cluster HA warning | Based on event com.vmware.vc.HA.InvalidMaster. | Warning | Manual | There is an issue with VMware high-availability protection for this cluster. |
| Based on event com.vmware.vc.HA.UserHeartbeatDatastoreRemoved. |
| Based on event com.vmware.vc.HA.VcCannotFindMasterEvent. |
| Based on event com.vmware.vc.HA.HostPartitionedFromMasterEvent. |
| Based on event com.vmware.vc.HA.HostUnconfiguredWithProtectedVms. |
| Based on event com.vmware.vc.HA.HostUnconfigureError. |
| Based on event com.vmware.vc.HA.NotAllHostAddrsPingable. |

vCloud Director vApp

vCloud Director vApp

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| vApp health status | VMware Cloud Director object task status equals Warning. | Warning | Automatic | vApp health status has changed. |
| VMware Cloud Director object task status equals Alert. | Error |
| vApp runtime lease timeout | vApp runtime lease timeout is 14 days. | Warning | Automatic | vApp runtime lease has expired. Once a vApp is powered on for the first time, the clock starts for the Maximum Runtime Lease. The Maximum Runtime Lease is how long a vApp can be powered on before its automatically suspended. |
| vApp runtime lease timeout is 7 days. | Error |
| vApp storage lease timeout | vApp storage lease timeout is 14 days. | Warning | Automatic | vApp storage lease has expired. A vApp storage lease begins when a user stops the vApp. Storage leases do not affect running vApps. |
| vApp storage lease timeout is 7 days. | Error |

vCloud Director Organization

vCloud Director Organization

| Alarm Name | Rule Event | Severity | Resolve Action | Description |
| Organization blocking task number | Number of blocking tasks is 1 or more. | Warning | Automatic | Some tasks are in a pending state as a result of blocking. |
| Number of blocking tasks is 5 or more. | Error |
| Organization blocking task timeout | Blocking tasks timeout is 5 minutes. | Warning | Automatic | One or more organization blocking tasks has expired. |
| Blocking tasks timeout is 10 minutes. | Error |

vCloud Director Org VDC

vCloud Director Org VDC

| Alarm Name | Rule Event | Severity | Resolve Action | Description |
| Network pool usage | Network pool usage is above 90%. | Warning | Automatic | Network pool usage has exceeded the configured threshold. |
| Network pool usage is above 95%. | Error |
| Org VDC CPU usage | Average CPU usage for 15 minutes is above 80%. | Warning | Automatic | Organization VDC has exceeded the CPU usage threshold. |
| Average CPU usage for 15 minutes is above 90%. | Error |
| Org VDC health status | VMware Cloud Director object task status equals Warning. | Warning | Automatic | Organization VDC health status has changed. |
| VMware Cloud Director object task status equals Alert. | Error |
| Org VDC memory usage | Average memory usage for 15 minutes is above 80%. | Warning | Automatic | Organization VDC has exceeded the memory usage threshold. |
| Average memory usage for 15 minutes is above 90%. | Error |
| Org VDC storage usage | Average storage usage for 15 minutes is above 80%. | Warning | Automatic | Organization VDC has exceeded the storage usage threshold. |
| Average storage usage for 15 minutes is above 90%. | Error |

vCloud Director Provider VDC

vCloud Director Provider VDC

| Alarm Name | Rule Event | Severity | Resolve Action | Description |
| Provider VDC CPU usage | Average CPU usage for 15 minutes is above 80%. | Warning | Automatic | Provider VDC has exceeded the threshold for CPU Usage |
| Average CPU usage for 15 minutes is above 90%. | Error |
| Provider VDC health status | VMware Cloud Director object task status equals Warning. | Warning | Automatic | Provider VDC health status has changed. |
| VMware Cloud Director object task status equals Alert. | Error |
| Provider VDC memory usage | Average memory usage for 15 minutes is above 80%. | Warning | Automatic | Provider VDC has exceeded the memory usage threshold. |
| Average memory usage for 15 minutes is above 90%. | Error |
| Provider VDC storage usage | Average storage usage for 15 minutes is above 80%. | Warning | Automatic | Provider VDC has exceeded the storage usage threshold. |
| Average storage usage for 15 minutes is above 90%. | Error |


