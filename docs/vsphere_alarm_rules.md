---
title: "Alarm Rules for VMware vSphere"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vsphere_alarm_rules.html"
last_updated: "11/5/2024"
product_version: "13.0.1.6168"
---

# Alarm Rules for VMware vSphere


Veeam ONE offers the following types of alarm rules for VMware vSphere infrastructure objects.

vCenter Server

vCenter Server

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some vCenter-related event is generated. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Power or connection state changes | An alarm is triggered if the vCenter Server state reports to be equal or not equal to a specific state value (for example, if vCenter Server is not responding). |

Cluster

Cluster

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some cluster-related event is generated. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified threshold value (for example, if the memory usage exceeds 80%). |

Host

Host

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some host-related event is generated. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Hardware sensor state changes | An alarm is triggered if the sensor state reports to be equal or not equal to a specific state value (Normal, Warning, Alert, Unknown). |
| Number of VMs is out of allowed range | An alarm is triggered if the number of running, powered off or suspended VMs on the ESXi host is above or below the specified threshold value. This type of alarm can be configured if it is necessary to limit the number of VMs running on the ESXi host at the same time to avoid the host overload. |
| Power or connection state changes | An alarm is triggered if the host state reports to be equal or not equal to a specific state value (for example, if the ESXi host is not responding). |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified threshold value (for example, if the CPU usage exceeds 75%). |

Resource Pool

Resource Pool

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some event is generated on a resource pool. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified value (for example, if the CPU usage exceeds 80%). |

Virtual Machine

Virtual Machine

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some VM-related event is generated (for example, if the MAC address of the VM conflicts with the MAC address of another VM existing in the virtual infrastructure). |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Guest disk space | An alarm is triggered if available disk space on guest volumes is above or below the specified threshold value. You can choose to specify the amount of due free space as an absolute value or a relative value. For example, an alarm is triggered if free disk space falls below 1 GB or 10% of total space. |
| Heartbeat is missing | An alarm is triggered if a monitored virtual machine is not available or overloaded for a specific period of time (for example, if heartbeat is missing for 5 minutes). |
| Number of running services | [For Windows-based machines] An alarm is triggered if the number of services running on a VM is greater than the specified threshold. |
| Orphaned Veeam Backup & Replication snapshot | An alarm is triggered if a VM has a snapshot that Veeam Backup & Replication created (to back up, replicate or perform another data protection operation for the VM) but was unable to remove when the operation was over. |
| Power or connection state changes | An alarm is triggered if the state of the VM reports to be equal or not equal to the specified state value (for example, if the VM is suspended). |
| Process performance | [For Windows-based machines] An alarm is triggered if the specified counter for a VM process is above or below the specified value (for example, if the CPU usage by a process exceeds 15%). |
| Process state | [For Windows-based machines] An alarm is triggered if VM process state is equal or not equal to a specific state value (Terminated, Running). |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified value (for example, if the CPU ready level exceeds 5%). |
| Service state | [For Windows-based machines] An alarm is triggered if service state is equal or not equal to a specific state value (Running, Paused, Stopped). |
| Snapshot age for VM | An alarm is triggered if the current snapshot is older than a specified number of hours. This rule helps monitor forgotten snapshots that are consuming valuable storage space and degrading performance of virtual machines. |
| Snapshot size for VM | An alarm is triggered if the size of the VM snapshot is above or below the specified threshold value. You can choose to specify the size of the snapshot as an absolute value or a relative value. For example, an alarm is triggered if the snapshot size exceeds 5 GB or 10% of total available disk space. |
| VM snapshots number has exceeded the configured threshold | An alarm is triggered if the number of snapshots created for the VM is greater than the specified threshold. |
| VMware VM tools state changes | An alarm is triggered if the state of the VMware Tools reports to be equal or not equal to the specified state value (for example, if the VMware Tools is out of date). |
| VMs with no restore points | An alarm is triggered if the age of the latest backup or replica restore point for the VM has exceeded the threshold (that is, if there are no restore points for the specified RPO period). |

Datastore

Datastore

| Rule Type | Description |
| Datastore is running out of free space | An alarm is triggered if free space on the datastore is above or below the specified threshold value. You can choose to specify the free space threshold as an absolute value or a relative value. For example, an alarm is triggered if the datastore space falls below 10 GB or 15% of total space. |
| Datastore performance | An alarm is triggered if a performance counter of a datastore is above or below the specified threshold value. |
| Datastore provisioned space | An alarm is triggered if the provisioned disk space is above or below the specified threshold value. You can select to specify the threshold as an absolute value or a relative value. For example, an alarms is triggered if the provisioned disk space exceeds 500 GB or 400% compared to the datastore capacity. |
| Event-based rule | An alarm is triggered if some datastore-related event is generated. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Power or connection state changes | An alarm is triggered if the state of the datastore reports to be equal or not equal to the specified state value (for example, if the datastore is not accessible). |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified threshold value (for example, if the datastore I\O threshold is violated). |

Any Object

Any Object

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some event is generated on any object in the infrastructure. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |

vCloud Director vApp

vCloud Director vApp

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some vApp-related event in generated. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified value (for example, if the storage usage exceeds 80%). |
| System health status change | An alarm is triggered if the object health state changes. |
| vApp runtime lease timeout | An alarm is triggered in N days after the vApp runtime lease has expired. |
| vApp storage lease timeout | An alarm is triggered in N days after the vApp storage lease has expired. |
| vCloud Director object task status | An alarm is triggered if the vApp state reports to be equal or not equal to a specific state value (for example, if warnings are registered for the vApp). |

vCloud Director Organization

vCloud Director Organization

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some event is generated on the organization. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Organization VDC blocking task number | An alarm is triggered if the number of pending blocking tasks has exceeded the specified threshold. |
| Organization VDC blocking task timeout | An alarm is triggered in N minutes after the blocking tasks has expired. |
| System health state change | An alarm is triggered if the object health state changes. |
| vCloud Director object task status | An alarm is triggered if the organization state reports to be equal or not equal to a specific state value (for example, if warnings are registered for the organization). |

vCloud Director Org VDC

vCloud Director Org VDC

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some event is generated on the organization VDC. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Network pool is running out of available IP addresses | An alarm is triggered if the number of remaining IP addresses is above or below the specified threshold value. You can select to specify the threshold as an absolute value or a relative value. For example, if the number of remaining IP addresses is lower than 5 or 10% of the total number for the organization VDC network. |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified value (for example, if the CPU ready level exceeds 5%). |
| System health status change | An alarm is triggered if the object health state changes. |
| vCloud Director object task status | An alarm is triggered if the organization VDC state reports to be equal or not equal to a specific state value (for example, if warnings are registered for the organization VDC). |

vCloud Director Provider VDC

vCloud Director Provider VDC

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some event is generated on the provider VDC. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified value (for example, if the storage usage exceeds 80%). |
| System health status change | An alarm is triggered if the object health state changes. |
| vCloud Director object task status | An alarm is triggered if the provider VDC state reports to be equal or not equal to a specific state value (for example, if warnings are registered for the provider VDC). |


