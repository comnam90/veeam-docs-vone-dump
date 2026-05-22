---
title: "Object Properties"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/properties.html"
last_updated: "5/19/2026"
product_version: "13.0.1.6168"
---

# Object Properties


To create grouping expressions, you can use properties of the following types of objects:

* [Host](properties.md#host)
* [Storage](properties.md#storage)
* [Cluster](properties.md#cluster)
* [Virtual Machine](properties.md#vm)
* [Computer](properties.md#agent)
* [Enterprise Application](#app)

Host

The following properties of host systems are supported in grouping expressions.

Host

| Property | Return Data Type | Description |
| CustomAttribute | Text (string) | Returns a value of a custom attribute assigned to a host.  Specify the name of a custom attribute in brackets. For example, CustomAttribute("department") will return the value of the 'department' attribute for a host.  Note:   * This property is available for VMware vSphere hosts only. * You cannot use methods to define the custom attribute name. However, the CustomAttribute property can be used to define values in methods. |
| CustomProperty | Text (string) | Returns a value of a custom property assigned to a host.  Specify the name of a custom property in brackets. For example, CustomProperty("department") will return the value of the 'department' property for a host.  Note: This property is available for Microsoft Hyper-V hosts only. |
| Tag | Text (string) | Returns a tag assigned to a host.  Specify the name of a tag category in brackets. For example, Tag("department") will return the tag of the 'department' category for a host.  Note: This property is available for VMware vSphere 5.5 or later. |
| Name | Text (string) | Returns a host name. |
| Memory | Numeric  (double precision floating-point number) | Returns an amount of host physical memory, in GB. |
| Location | Text (string) | Returns a location assigned to a host in Veeam Backup & Replication. |
| ProcessorCores | Numeric (integer) | Returns a number of processor cores for a host. |
| CPUFrequency | Numeric  (double precision floating-point number) | Returns a CPU frequency, in MHz. |
| VMCount | Numeric (integer) | Returns a number of VMs registered on a host. |
| Datacenter | Text (string) | Returns a name of a datacenter. |
| HostModel | Text (string) | Returns a host model.  Note: This property is available for VMware vSphere hosts only. |
| CPUSockets | Numeric (integer) | Returns a number of CPU sockets for a host. |
| InfrastructureLocation | Text (string) | Returns a path to a host in the virtual infrastructure. |
| Connection\_State | Text (string) | Returns a connection state of a host. |
| PowerState | Text (string) | Returns a power state of a host. |

Storage

The following properties of storage systems are supported in grouping expressions.

Storage

| Property | Return Data Type | Description |
| CustomAttribute | Text (string) | Returns a value of a custom attribute assigned to a storage.  Specify the name of a custom attribute in brackets. For example, CustomAttribute("department") will return the value of the 'department' attribute for a storage.  Notes:   * This property is available for VMware vSphere storage systems only. * You cannot use methods to define the custom attribute name. However, the CustomAttribute property can be used to define values in methods. |
| Tag | Text (string) | Returns a tag assigned to a storage.  Specify the name of a tag category in brackets. For example, Tag("department") will return the tag of the 'department' category for a storage.  Note: This property is available for VMware vSphere 5.5 or later. |
| Name | Text (string) | Returns a storage object name. |
| Capacity | Numeric  (double precision floating-point number) | Returns storage capacity, in GB. |
| FileSystemType | Text (string) | Returns a type of storage file system, such as VMFS or NTFS. |
| FreeSpace | Numeric  (double precision floating-point number) | Returns an amount of free storage space, in GB. |
| UsedSpace | Numeric  (double precision floating-point number) | Returns an amount of used storage space, in GB. |
| VMCount | Numeric (integer) | Returns a number of VMs whose files reside on a storage object. |
| Type | Text (string) | Returns a storage type (Shared or Local). |
| InfrastructureLocation | Text (string) | Returns a path to a storage object in the virtual infrastructure. |
| Datacenter | Text (string) | Returns a name of a datacenter. |
| DatastoreCluster | Text (string) | Returns a name of a cluster where storage object resides.  Note: This property is available for VMware vSphere storage objects only. |

Cluster

The following properties of clusters are supported in grouping expressions.

Cluster

| Property | Return Data Type | Description |
| CustomAttribute | Text (string) | Returns a value of a custom attribute assigned to a cluster.  Specify the name of a custom attribute in brackets. For example, CustomAttribute("department") will return the value of the 'department' attribute for a cluster.  Notes:   * This property is available for VMware vSphere clusters only. * You cannot use methods to define the custom attribute name. However, the CustomAttribute property can be used to define values in methods. |
| CustomProperty | Text (string) | Returns a value of a custom property assigned to a cluster.  Specify the name of a custom property in brackets. For example, CustomProperty("department") will return the value of the 'department' property for a cluster.  Note: This property is available for Microsoft Hyper-V clusters only. |
| Tag | Text (string) | Returns a tag assigned to a cluster.  Specify a name of a tag category in brackets. For example, Tag("department") will return the tag of the 'department' category for a cluster.  Note: This property is available for VMware vSphere 5.5 or later. |
| Name | Text (string) | Returns a cluster name. |
| CPUFrequency | Numeric (integer) | Returns cluster CPU frequency, in MHz. |
| Connection\_State | Text (string) | Returns a connection state of a cluster.  Note: This property is available for Microsoft Hyper-V clusters only. |
| Datacenter | Text (string) | Returns a name of a datacenter. |
| HostCount | Numeric (integer) | Returns a number of hosts in a cluster. |
| Memory | Numeric (integer) | Returns a memory size of a cluster, in MB. |
| ProcessorCores | Numeric (integer) | Returns a sum of cores for all hosts in a cluster. |
| VMCount | Numeric (integer) | Returns a number of VMs whose files reside in a cluster. |
| InfrastructureLocation | Text (string) | Returns a path to a cluster in the virtual infrastructure. |
| IsDRSEnabled | Text (string) | Returns a flag that indicates if distributed resource scheduler enabled in a cluster.  Note: This property is available for VMware vSphere clusters only. |
| Location | Text (string) | Returns a location assigned to a host in Veeam Backup & Replication. |

Virtual Machine

The following properties of VMs are supported in grouping expressions.

Virtual Machine

| Property | Return Data Type | Description |
| BackupJob | Text (string) | Returns a name of a backup job that protects a VM. |
| BackupRPO | Numeric (integer) | Returns the number of hours that passed since last backup session completed. |
| CheckpointCreateTime | Date and time | Returns the date and time when a checkpoint was created, in the mm/dd/yyyy hh:mm:ss format.  Notes:   * This property is available for Microsoft Hyper-V VMs only. * If a VM has several checkpoints, the property returns the creation date of the current checkpoint. |
| ComputerName | Text (string) | Returns a domain name assigned to a VM. |
| Connection\_State | Text (string) | Returns a connection state of a VM. |
| CustomAttribute | Text (string) | Returns a value of a custom attribute assigned to a VM.  Specify the name of a custom attribute in brackets. For example, CustomAttribute("department") will return the value of the 'department' attribute for a VM.  Notes:   * This property is available for VMware vSphere VMs only. * You cannot use methods to define the custom attribute name. However, the CustomAttribute property can be used to define values in methods. |
| CustomProperty | Text (string) | Returns a value of a custom property assigned to a VM.  Specify the name of a custom property in brackets. For example, CustomProperty("department") will return the value of the 'department' property for a VM.  Note: This property is available for Microsoft Hyper-V VMs only. |
| CPUFrequency | Numeric  (double precision floating-point number) | Returns a frequency of a CPU in MHz.  Note: This property is available for Microsoft Hyper-V VMs only. |
| Datacenter | Text (string) | Returns a name of a datacenter where a VM resides. |
| Datastore | Text (string) | Returns the name of a storage system (datastore) where VM files reside.  Note: If VM files reside on several datastores, the property returns the name of a datastore where the VM configuration file is located. |
| GuestOS | Text (string) | Returns a VM guest OS. |
| HasBackups | Text (string) | Returns a flag indicating whether a VM has backups or not (Yes, No). |
| HasSnapshots | Text (string) | Returns a flag indicating whether a VM has snapshots or not (Yes, No).  Note: This property is available for VMware vSphere VMs only. |
| HasCheckpoints | Text (string) | Returns a flag indicating whether a VM has checkpoints or not (Yes, No).  Note: This property is available for Microsoft Hyper-V VMs only. |
| Host | Text (string) | Returns a name of a host on which a VM resides. |
| InfrastructureLocation | Text (string) | Returns a path to a VM in the virtual infrastructure. |
| IpAddress | Text (string) | Returns an IP address assigned to a VM. |
| IsReplica | Text (string) | Returns a flag indicating whether a VM is a replica of an original VM. |
| IsShielded | Text (string) | Returns a flag indicating whether a VM is shielded.  Note: This property is available for Microsoft Hyper-V VMs only. |
| LastBackupDate | Date and time | Returns the date and time when the latest backup session was performed for a VM in Veeam Backup & Replication, in the mm/dd/yyyy hh:mm:ss format.  Note: The backup session is returned only if a restore point was created as a result of this session. |
| Location | Text (string) | Returns a location assigned to a VM in Veeam Backup & Replication. |
| Memory | Numeric  (double precision floating-point number) | Returns the amount of memory allocated to a VM. |
| Name | Text (string) | Returns a VM name. |
| Network | Text (string) | Returns the network to which a VM is connected.  Note: If a VM is connected to several networks, the property will return a random network. |
| PowerState | Text (string) | Returns a VM power state.   * For VMware vSphere: Powered On, Powered Off, Suspended  * For Microsoft Hyper-V: Powered Off, Running, Saved |
| ReplicationJob | Text (string) | Returns a name of a replication job in which a VM is included in Veeam Backup & Replication.  Note: If a VM is included in several replication jobs, the property will return a random job. |
| ReplicationRPO | Numeric (integer) | Returns the number of hours that passed since last replication session completed. |
| SnapshotAge | Numeric (integer) | Returns how many hours ago a snapshot was created.  Note: This property is available for VMware vSphere VMs only. |
| SnapshotCreateTime | Date and time | Returns the date and time when a snapshot was created, in the mm/dd/yyyy hh:mm:ss format.  Notes:   * This property is available for VMware vSphere VMs only. * If a VM has several snapshots, the property returns the creation date of the latest snapshot. |
| Tag | Text (string) | Returns a tag assigned to a VM.  Specify the name of a tag category in brackets. For example, Tag("department") will return the tag of the 'department' category for a VM.  Note: This property is available for VMware vSphere 5.5 or later. |
| vCPU | Numeric (integer) | Returns the number of vCPUs configured for a VM. |
| VirtualDiskSize | Numeric  (double precision floating-point number) | Returns the amount space occupied by all VM disks. |
| VMFolder | Text (string) | Returns a name of a folder where VM files reside.  Note: This property is available for VMware vSphere VMs only. |
| VMFolderPath | Text (string) | Returns a user path to a VM in the virtual infrastructure.  Note: This property is available for VMware vSphere VMs only. |

Computer

The following properties of protected computers are supported in grouping expressions.

Computer

| Property | Return Data Type | Description |
| BackupServer | Text (string) | Returns a name of Veeam Backup & Replication server that manages the backup agent. |
| LastBackupDate | Date and time | Returns the date and time when the latest backup session was performed for a computer in Veeam Backup & Replication, in the mm/dd/yyyy hh:mm:ss format. |
| BackupRPO | Numeric (integer) | Returns a number of hours that passed since last backup session completed. |
| BpAgentLicenseType | Text (string) | Returns a type of license installed on a backup agent. |
| Location | Text (string) | Returns a location assigned to a computer in Veeam Backup & Replication. |
| BpAgentManagementType | Text (string) | Returns a management type of a backup agent (Standalone, Managed by VBR). |
| Name | Text (string) | Returns a name of a computer that runs a backup agent. |
| ProtectedComputersGroup | Text (string) | Returns a name of a protection group for a computer. |
| ClusterName | Text (string) | Returns a name of a failover cluster in which a computer resides. |
| IpAddress | Text (string) | Returns an IP address assigned to a computer that runs a backup agent. |
| FQDN | Text (string) | Returns an FQDN assigned to a computer that runs a backup agent. |
| JobName | Text (string) | Returns a name of a job that runs on a backup agent. |
| PolicyName | Text (string) | Returns a name of a backup policy assigned to a backup agent. |

Enterprise Application

The following properties of protected enterprise applications are supported in grouping expressions.

Enterprise Application

| Property | Return Data Type | Description |
| ApplicationPolicyName | Text (string) | Returns a name of a backup policy configured for an application. |
| BackupRPO | Numeric (integer) | Returns a number of hours that passed since last backup session completed. |
| BackupServer | Text (string) | Returns a name of Veeam Backup & Replication server that manages the application plug-in. |
| FQDN | Text (string) | Returns an FQDN assigned to a server that runs a protected application. |
| HasDataBackupSessions | Text (string) | Returns a flag indicating whether an application has backup policies configured or not (Yes, No). |
| IpAddress | Text (string) | Returns an IP address assigned to a server that runs a protected application. |
| LastBackupDate | Date and time | Returns the date and time when the latest backup session was performed for an application in Veeam Backup & Replication, in the mm/dd/yyyy hh:mm:ss format. |
| Location | Text (string) | Returns a location assigned to an application server in Veeam Backup & Replication. |
| Name | Text (string) | Returns a name of a server that runs an application. |
| ProtectionGroup | Text (string) | Returns a name of a protection group for an applications. |


