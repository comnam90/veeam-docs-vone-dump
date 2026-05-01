---
title: "Microsoft Hyper-V Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/hyperv_alarms_events.html"
last_updated: "4/29/2026"
product_version: "13.0.1.6168"
---

# Microsoft Hyper-V Alarms


This section describes predefined alarms for Microsoft Hyper-V infrastructure components.

Host

Host

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Bad Hyper-V username logon attempt | Based on event 4625 Microsoft-Windows-Security-Auditing. | Error | Manual | This event records a failed user logon attempt. The combination of username, password and permissions is the mechanism by which Hyper-V server authenticate a user for access and authorize the user to perform activities. |
| Cluster communication session failed | Based on event 1570 Microsoft-Windows-FailoverClustering. | Error | Manual | Host mode failed to establish a communication session while joining the cluster. |
| Cluster host node network connectivity error | Based on event 1554 Microsoft-Windows-FailoverClustering. | Error | Manual | This cluster node has no network connectivity. It cannot participate in the cluster until connectivity is restored. |
| Cluster hosts update version mismatch | Based on event 1548 Microsoft-Windows-FailoverClustering. | Error | Manual | Host node has established a communication session with another node and detected that it is running a different but compatible version of the cluster service software. |
| Cluster network failure | Based on event 1127 Microsoft-Windows-FailoverClustering. | Warning | Manual | Cluster network interface for cluster node has failed. |
| Cluster witness resource failure | Based on event 1558 Microsoft-Windows-FailoverClustering. | Error | Manual | The cluster service detected a problem with the witness resource. The witness resource will be failed over to another node within the cluster in an attempt to reestablish access to cluster configuration data. |
| Cluster witness resource update failure | Based on event 1557 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster service failed to update the cluster configuration data on the witness resource. |
| Host available memory | Average Hyper-V Services memory usage for 15 minutes is above 80%. | Warning | Automatic | This host is low on available memory. |
| Average Hyper-V Services memory usage for 15 minutes is above 90%. | Error |
| Host average disk queue length | Average disk queue length for 15 minutes is above 1. | Warning | Automatic | Average disk queue length on the host may report on too many I/O requests. This means that not all requests are queued. Some requests are completed and are on their way back to where the performance data is being collected. |
| Average disk queue length for 15 minutes is above 2. | Error |
| Host average memory pressure | Average pressure for 15 minutes is above 90%. | Warning | Automatic | This host has exceeded the threshold for memory pressure. |
| Average pressure for 15 minutes is above 100%. | Error |
| Host cluster membership | Based on event 1093 Microsoft-Windows-FailoverClustering. | Error | Manual | The Cluster service cannot identify host node as a member of failover cluster. |
| Host connection failure | State not equals Connected for 5 minutes or more. | Error | Automatic | This alarm monitors Hyper-V host connection state. |
| Host CPU time per dispatch | Average host CPU wait time for 15 minutes is 60 microseconds. | Warning | Automatic | The counter shows the average time Virtual Machines running on the host spent waiting for a virtual processor to be dispatched onto a logical processor. More vCPUs on host means more things the dispatcher has to schedule thus wait time raises. |
| Average host CPU wait time for 15 minutes is 100 microseconds. | Error |
| Host CPU usage | Average Total Run Time value for 15 minutes is above 75%. | Warning | Automatic | This host has exceeded the threshold for CPU usage. |
| Average Total Run Time value for 15 minutes is above 85%. | Error |
| Host failed to form a cluster | Based on event 1546 Microsoft-Windows-FailoverClustering. | Error | Manual | Host node failed to form a failover cluster. |
| Host Image Management service is not running | \*Hyper-V Image Management\* service is not running for 5 minutes or more. | Error | Automatic | The service required to manage virtual storage is not running. No virtual storage management operations can be performed. |
| Host Memory Pages Usage | Average pages/sec value for 15 minutes is above 500. | Warning | Automatic | The counter shows the rate at which pages are read from or written to disk to resolve hard page faults. This counter is a primary indicator of the types of faults that cause system-wide delays. |
| Average pages/sec value for 15 minutes is above 1500. | Error |
| Host network average output queue length | Average network output queue length for 15 minutes is above 1. | Warning | Automatic | This host has exceeded the threshold for the length of the queue in packets. This counter should be 0 at all times. |
| Average network output queue length for 15 minutes is above 2. | Error |
| Host network outbound errors number | Average network outbound errors number for 15 minutes is above 1. | Warning | Automatic | This host has exceeded the threshold for the outbound packets that couldn't be transmitted because of errors. |
| Average network outbound errors number for 15 minutes is above 2. | Error |
| Host Networking Management service is not running | \*Hyper-V Networking Management\* service is not running for 5 minutes or more. | Error | Automatic | The Hyper-V Networking Management Service is not configured to start automatically. Virtual networks cannot be managed until the service is started. |
| Host node failed to form a cluster | Based on event 1573 Microsoft-Windows-FailoverClustering. | Error | Manual | Host node failed to form a cluster. |
| Host node failed to join cluster | Based on event 1572 Microsoft-Windows-FailoverClustering. | Error | Manual | Host node failed to join the cluster because it could not send and receive failure detection network messages with other cluster nodes. |
| Host node was evicted from cluster | Based on event 1011 Microsoft-Windows-FailoverClustering. | Warning | Manual | Cluster host node has been evicted from the failover cluster. |
| Host node was removed from cluster | Based on event 1135 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster node was removed from the active failover cluster membership. If the Cluster service fails to start on a failover cluster node, the node cannot function as part of the cluster. |
| Host restart | Based on event 1074 User32. | Information | Automatic | Host operation system has been restarted or shut down. |
| Missing latest cluster configuration data | Based on event 1561 Microsoft-Windows-FailoverClustering. | Error | Manual | The cluster service has determined that this node does not have the latest copy of cluster configuration data. Therefore, the cluster service has prevented itself from starting on this node. |
| Network communication failure | Based on event 1592 Microsoft-Windows-FailoverClustering. | Warning | Manual | Cluster node lost communication with another cluster node. Network communication was reestablished. |
| Unreachable cluster network interface | Based on event 1126 Microsoft-Windows-FailoverClustering. | Warning | Manual | Cluster network interface for cluster node is unreachable by at least one other cluster node attached to the network. |
| Virtual Machine Management service is not running | \*Hyper-V Virtual Machine Management\* service is not running. | Error | Automatic | The service required to manage virtual machines is not running. No virtual machine management operations can be performed. |

Virtual Machine

Virtual Machine

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Background disk merge failed | Based on event 19100 Microsoft-Windows-Hyper-V-VMMS. | Warning | Manual | The parent virtual hard disks associated with this virtual machine may be in an inconsistent state. |
| Background disk merge interruption | Based on event 19090 Microsoft-Windows-Hyper-V-VMMS. | Warning | Manual | The snapshot merge operation was interrupted. |
| Checkpoint configuration is not accessible | Based on event 16420 Microsoft-Windows-Hyper-V-VMMS. | Error | Manual | The configuration of checkpoint is no longer accessible. |
| Current memory pressure | Average memory pressure for 15 minutes is above 110%. | Warning | Automatic | This VM has exceeded the threshold for memory pressure. |
| Average memory pressure for 15 minutes is above 125%. | Error |
| Failed to assign dynamic MAC address | Based on event 12572 Microsoft-Windows-Hyper-V-SynthNic. | Error | Manual | Dynamic MAC address for VM network adapter was not assigned. |
| Failed to create memory contents file | Based on event 3320 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | Failed to create memory contents file. |
| Failed to create VM saved state file | Based on event 3080 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | Failed to create or access VM saved state file. |
| Failed to delete VM directory | Based on event 16150 Microsoft-Windows-Hyper-V-VMMS. | Warning | Manual | Cannot delete VM directory. |
| Failed to initialize VM memory | Based on event 3050 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | Failed to initialize VM memory. |
| Failed to merge virtual disk | Based on event 16210 Microsoft-Windows-Hyper-V-VMMS. | Warning | Manual | Cannot merge disk file on deletion. As a result, this disk may be in an inconsistent state. |
| Failed to power on VM | Based on event 12010 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | Failed to power on VM. |
| Based on event 12030 Microsoft-Windows-Hyper-V-Worker. |
| Based on event 12040 Microsoft-Windows-Hyper-V-Worker. |
| Based on event 12050 Microsoft-Windows-Hyper-V-Worker. |
| Failed to restore VM | Based on event 12080 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | Failed to restore a VM. |
| Failed to save VM | Based on event 12054 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | Failed to save state for a VM. |
| Guest disk space | Guest disk free space is below 10%. | Warning | Automatic | Guest OS volume is low on available guest disk space. |
| Guest disk free space is below 5%. | Error |
| Incompatible version of integration services | Based on event 4010 Microsoft-Windows-Hyper-V-Integration. | Warning | Manual | The version of a component of integration services is incompatible with another version. |
| Insufficient disk space | Based on event 16050 Microsoft-Windows-Hyper-V-VMMS. | Warning | Manual | Hyper-V disk space is low on available free space. |
| Invalid static MAC address | Based on event 12560 Microsoft-Windows-Hyper-V-SynthNic. | Error | Manual | By default, new virtual machines in Hyper-V are created with NICs that are assigned dynamic MAC addresses. |
| Based on event 12560 Microsoft-Windows-Hyper-V-Worker. |
| Based on event 12560 Microsoft-Windows-Hyper-V-VMMS. |
| Latest checkpoint age | VM checkpoint age is 48 hours or more. | Warning | Automatic | The age of the latest checkpoint for this VM has exceeded the configured threshold. |
| Latest checkpoint size | Hyper-V VM checkpoint size is above 10% of the VM size. | Warning | Automatic | The size of the latest checkpoint file for this VM has exceeded the configured threshold. |
| Hyper-V VM checkpoint size is above 20% of the VM size. | Error |
| Machine remoting system failure | Based on event 12480 Microsoft-Windows-Hyper-V-Worker. | Warning | Manual | Failure in machine remoting system has been detected. |
| No disk space to run this VM | Based on event 16060 Microsoft-Windows-Hyper-V-VMMS. | Error | Manual | VM has been paused because it has run out of disk space. |
| Not enough memory to start a VM | Based on event 3122 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | Hyper-V was unable to allocate RAM resources to start this VM. |
| Based on event 3030 Microsoft-Windows-Hyper-V-Worker. |
| Possible ransomware activity | Total Run Time is above 70%  and Virtual Storage Write is above 40 MB/s  or  Virtual Network Bytes Sent/sec is above 40 MB/s for 5 minutes. | Warning | Automatic | Veeam ONE detected suspicious activity on this VM. |
| Total Run Time is above 80%  and  Virtual Storage Write is above 60 MB/s  or Virtual Network Bytes Sent/sec is above 60 MB/s for 5 minutes. | Error |
| Static MAC address conflict | Based on event 12562 Microsoft-Windows-Hyper-V-SynthNic. | Warning | Manual | By default, new virtual machines in Hyper-V are created with NICs that are assigned dynamic MAC addresses. |
| Based on event 12562 Microsoft-Windows-Hyper-V-Worker. |
| Unexpected VM error | Based on event 16020 Microsoft-Windows-Hyper-V-VMMS. | Error | Manual | This VM has encountered an unexpected error. |
| VM configuration is not accessible | Based on event 16410 Microsoft-Windows-Hyper-V-VMMS. | Error | Manual | The configuration of virtual machine is no longer accessible. |
| Based on event 16400 Microsoft-Windows-Hyper-V-VMMS. |
| VM configuration module error | Based on event 4096 Microsoft-Windows-Hyper-V-Config. | Error | Manual | The VM configuration is no longer accessible. |
| VM CPU usage | Average guest run time for 15 minutes is above 75%. | Warning | Automatic | This VM has exceeded the threshold for CPU usage. |
| Average guest run time for 15 minutes is above 85%. | Error |
| VM disk errors | Average number of errors/min for 15 minutes is above 4. | Warning | Automatic | This VM has logged one or more errors that have occurred on its virtual device. |
| Average number of errors/min for 15 minutes is above 8. | Error |
| VM guest OS reboot | Based on event 18514 Microsoft-Windows-Hyper-V-Worker. | Information | Warning | Virtual Machine was rebooted. This warning is applied only to Windows Server 2012 and Windows Server 2012 R2. |
| VM initialization error | Based on event 3040 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | VM initialization has failed. |
| VM power status | State not equals Running for 5 minutes or more. | Error | Automatic | VM power state has been changed. |
| VM invalid switch port reference | Based on event 12570 Microsoft-Windows-Hyper-V-SynthNic. | Error | Manual | The virtual machine cannot be started. |
| VM restart | Based on event 18512 Microsoft-Windows-Hyper-V-Worker. | Information | Automatic | Virtual Machine was rebooted. This warning is applied only to Windows Server 2012 and Windows Server 2012 R2. |
| VM shutdown by guest | Based on event 18508 Microsoft-Windows-Hyper-V-Worker. | Information | Automatic | Virtual Machine was shut down. This warning is applied only to Windows Server 2012 and newer Windows server versions. |
| VM shutdown by host | Based on event 18504 Microsoft-Windows-Hyper-V-Worker. | Information | Automatic | Virtual Machine was shut down. This warning is applied only to Windows Server 2012 and newer Windows server versions. |
| VM vCPU time per dispatch | Average CPU wait time for 15 minutes is above 60 microseconds. | Warning | Automatic | The counter shows the average time spent waiting for a virtual processor to be dispatched onto a logical processor. |
| Average CPU wait time for 15 minutes is above 100 microseconds. | Error |
| VM with no backups | No backup restore points for the past 24 hours. | Warning | Automatic | This VM has not been backed up within the defined RPO (Recovery Point Objective) interval. |
| VM with no replica | No replica restore points for the past 24 hours. | Warning | Automatic | This VM has not been replicated within the defined RPO (Recovery Point Objective) interval. |
| VSS checkpoint failure | Based on event 10102 Microsoft-Windows-Hyper-V-VMMS. | Error | Manual | Failed to create the backup of virtual machine. |
| Based on event 15252 Microsoft-Windows-Hyper-V-VMMS. | Error |

Cluster

Cluster

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Cluster configuration data is missing or corrupt | Based on event 1575 Microsoft-Windows-FailoverClustering. | Error | Manual | An attempt to forcibly start the cluster service has failed because the cluster configuration data on host node is either missing or corrupt. |
| Cluster configuration database cannot be unloaded | Based on event 1593 Microsoft-Windows-FailoverClustering. | Error | Manual | The failover cluster database could not be unloaded and any potentially incorrect changes in memory could not be discarded. The cluster service will attempt to repair the database by retrieving it from another cluster node. |
| Cluster database could not be loaded | Based on event 1057 Microsoft-Windows-FailoverClustering. | Error | Manual | The cluster database could not be loaded. Ensure that a good copy of the cluster configuration is available to the node. |
| Cluster memory overcommitment | Based on event VeeamHvClusterReserveStateOkEvent. | Resolve | Automatic | When placing a virtual machine in a failover cluster, the placement process calculates whether the new virtual machine will over-commit the cluster. If the action will over-commit the cluster, the alarm will trigger. |
| Based on event VeeamHvClusterReserveStateErrorEvent. | Error |
| Cluster network is down | Based on event 1130 Microsoft-Windows-FailoverClustering. | Warning | Manual | Cluster network is down. |
| Cluster resource cannot be brought online | Based on event 1207 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster network name resource cannot be brought online. The computer object associated with the resource could not be updated in domain. |
| Cluster resource failure | Based on event 1069 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster resource in clustered service or application has failed. |
| Cluster service cannot be started | Based on event 1090 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster service cannot be started. An attempt to read configuration data from the Windows registry failed. |
| Cluster service failed to start | Based on event 1105 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster service failed to start because it was unable to register interfaces with the RPC service. |
| Cluster service failed to write data to a file | Based on event 1080 Microsoft-Windows-FailoverClustering. | Warning | Manual | Cluster service could not write to a file. In a failover cluster, most clustered services or applications use at least one disk, also called a disk resource, that you assign when you configure the clustered service or application. Clients can use the clustered service or application only when the disk is functioning correctly. |
| Cluster service fatal error | Based on event 1000 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster service suffered an unexpected fatal error. |
| Cluster service interruption | Based on event 1006 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster service was halted due to incomplete connectivity with other cluster nodes. |
| Cluster service shut down | Based on event 1177 Microsoft-Windows-FailoverClustering. | Error | Manual | The Cluster service is shutting down because quorum was lost. |
| Cluster Shared Volume is not available | Based on event 5120 Microsoft-Windows-FailoverClustering. | Warning | Automatic | Cluster Shared Volume is no longer available on this node. All I/O will temporarily be queued until a path to the volume is reestablished. |
| Based on event 5122 Microsoft-Windows-FailoverClustering. | Resolve |
| Cluster Shared Volume is not directly accessible | Based on event 5121 Microsoft-Windows-FailoverClustering. | Warning | Automatic | Cluster Shared Volume is no longer directly accessible from this cluster node. I/O access will be redirected to the storage device over the network through the node that owns the volume. This may result in degraded performance. |
| Based on event 5122 Microsoft-Windows-FailoverClustering. | Resolve |
| Failed to bring cluster resource online | Based on event 1049 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster IP address resource cannot be brought online. |
| Failed to copy cluster configuration data file | Based on event 1581 Microsoft-Windows-FailoverClustering. | Warning | Manual | The restore request for the cluster configuration data failed to make a copy of the existing cluster configuration data file (ClusDB). |
| Failed to create cluster resource name in domain | Based on event 1193 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster network name resource failed to create its associated computer object in domain. |
| Failed to migrate virtual machine | Based on event 22506 Microsoft-Windows-Hyper-V-High-Availability. | Error | Manual | Live migration for this VM did not succeed. |
| Based on event 22505 Microsoft-Windows-Hyper-V-High-Availability. |
| Based on event 21100 Microsoft-Windows-Hyper-V-High-Availability. |
| Failed to unload failover cluster database | Based on event 1574 Microsoft-Windows-FailoverClustering. | Error | Manual | The failover cluster database could not be unloaded. |
| Inconsistency within the failover cluster | Based on event 1073 Microsoft-Windows-FailoverClustering. | Error | Manual | The Cluster service was halted to prevent an inconsistency within the failover cluster. |
| Invalid IP address detected | Based on event 1047 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster IP address resource cannot be brought online because the address value is invalid. |
| Invalid IP address for cluster resource | Based on event 1360 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster IP address resource failed to come online. |
| Invalid subnet mask detected | Based on event 1046 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster IP address resource cannot be brought online because the subnet mask value is invalid. |
| Unexpected cluster service problem | Based on event 1556 Microsoft-Windows-FailoverClustering. | Error | Manual | The cluster service encountered an unexpected problem and will be shut down. |

Cluster Shared Volume

Cluster Shared Volume

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Active filter drivers detected | Based on event 5125 Microsoft-Windows-FailoverClustering. | Warning | Manual | Cluster Shared Volume has identified one or more active filter drivers on this device stack that could interfere with CSV operations. I/O access will be redirected to the storage device over the network through another Cluster node. This may result in degraded performance. |
| Based on event 5126 Microsoft-Windows-FailoverClustering. |
| Cluster Shared Volume read latency | Average read latency for 15 minutes is above 40 milliseconds. | Warning | Automatic | Cluster Shared Volume has exceeded the configured threshold of total read latency. |
| Average read latency for 15 minutes is above 80 milliseconds. | Error |
| Cluster Shared Volume write latency | Average write latency for 15 minutes is above 40 milliseconds. | Warning | Automatic | Cluster Shared Volume has exceeded the configured threshold of total write latency. |
| Average write latency for 15 minutes is above 80 milliseconds. | Error |
| Cluster Shared Volume free space | Free space is below 10%. | Warning | Automatic | Cluster Shared Volume is low on available free space. |
| Free space is below 5%. | Error |
| Redirected access was turned on | Based on event 5136 Microsoft-Windows-FailoverClustering. | Warning | Manual | Cluster Shared Volume redirected access was turned on. Access to the storage device will be redirected over the network from all cluster nodes that are accessing this volume. This may result in degraded performance. |
| Volume snapshot preparation error | Based on event 1584 Microsoft-Windows-FailoverClustering. | Error | Manual | A backup application initiated a VSS snapshot on Cluster Shared Volume without properly preparing the volume for snapshot. This snapshot may be invalid and the backup may not be usable for restore operations. |

Local Storage

Local Storage

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Datastore read latency | Avg Disk sec/Read value for 15 minutes is 40 milliseconds. | Warning | Automatic | This host local disk has exceeded the threshold for total read latency. This performance monitor counter measures the amount of time that read operations take to respond to the operating system. |
| Avg Disk sec/Read value for 15 minutes is 80 milliseconds. | Error |
| Datastore write latency | Avg Disk sec/Write value for 15 minutes is 40 milliseconds. | Warning | Automatic | This host disk has exceeded the threshold for total write latency. This performance monitor counter measures the amount of time that write operations take to respond to the operating system. |
| Avg Disk sec/Write value for 15 minutes is 80 milliseconds. | Error |
| Local volume free space | Free space is below 10%. | Warning | Automatic | Local volume is low on available free space. |
| Free space is below 5%. | Error |

Any Hyper-V Object

Any Hyper-V Object

| Alarm Name | Event/Condition | Severity | Resolve Action | Description |
| Cluster Shared Volume is no longer accessible | Based on event 5142 Microsoft-Windows-FailoverClustering. | Error | Manual | Cluster Shared Volume is no longer accessible from this cluster node because of error. |
| Failed to load VM configuration | Based on event 16300 Microsoft-Windows-Hyper-V-VMMS. | Error | Manual | Cannot load a virtual machine configuration |
| Failed to open VM attachment | Based on event 12290 Microsoft-Windows-Hyper-V-Worker. | Error | Manual | Cannot open VM attachment. |
| Based on event 12290 Microsoft-Windows-Hyper-V-SynthStor. |
| Based on event 12290 Microsoft-Windows-Hyper-V-VMMS. |
| Based on event 12140 Microsoft-Windows-Hyper-V-VMMS. |
| Based on event 12140 Microsoft-Windows-Hyper-V-Worker. |
| Based on event 12140 Microsoft-Windows-Hyper-V-SynthStor. |
| Based on event 12240 Microsoft-Windows-Hyper-V-VMMS. |
| Based on event 12240 Microsoft-Windows-Hyper-V-Worker. |
| Based on event 12240 Microsoft-Windows-Hyper-V-SynthStor. |
| Failed to register VM configuration file | Based on event 20100 Microsoft-Windows-Hyper-V-VMMS. | Warning | Manual | The Hyper-V Virtual Machine Management service failed to register the configuration for the virtual machine. |
| Failed to revert to VSS snapshot | Based on event 10104 Microsoft-Windows-Hyper-V-VMMS. | Error | Manual | Failed to revert to VSS snapshot on one or more virtual hard disks of the virtual machine. |
| Failed to unregister VM configuration file | Based on event 20102 Microsoft-Windows-Hyper-V-VMMS. | Warning | Manual | The Hyper-V Virtual Machine Management service failed to unregister the configuration for the virtual machine. |
| Failed to verify VM configuration file | Based on event 20104 Microsoft-Windows-Hyper-V-VMMS. | Warning | Manual | The Hyper-V Virtual Machine Management service failed to verify that the configuration is registered for the virtual machine. |
| VM configuration file is corrupt | Based on event 16310 Microsoft-Windows-Hyper-V-VMMS. | Error | Manual | Cannot load the virtual machine because the configuration is corrupt. |


