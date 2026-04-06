---
title: "Alarm Rules for Microsoft Hyper-V"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/hyperv_alarm_rules.html"
last_updated: "3/18/2025"
product_version: "13.0.1.6168"
---

# Alarm Rules for Microsoft Hyper-V


Veeam ONE offers the following types of alarm rules for Microsoft Hyper-V infrastructure objects.

Host

Host

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some host-related event is generated. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Power or connection state changes | An alarm is triggered if the host state reports to be equal or not equal to a specific state value (for example, if the Hyper-V host is not responding). |
| Service state | An alarm is triggered if host service state is equal or not equal to a specified state value (Running, Paused, Stopped). |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified threshold value (for example, if the Total Run Time exceeds 75%). |
| Service state | An alarm is triggered if service state is equal or not equal to a specific state value (Running, Paused, Stopped). |

Virtual Machine

Virtual Machine

| Rule Type | Description |
| Checkpoint age for Hyper-V VM has exceeded the configured threshold | An alarm is triggered if the current checkpoint is older than a specified number of hours. This rule helps monitor forgotten checkpoints that are consuming valuable storage space and degrading performance of virtual machines. |
| Checkpoint size for Hyper-V VM is out of allowed range | An alarm is triggered if the size of the VM checkpoint is above or below the specified threshold value. You can choose to specify the size of the checkpoint as an absolute value or a relative value (for example, if the checkpoint size exceeds 10% of total available disk space). For example, if the checkpoint size exceeds 5 GB or 10% of total disk space. |
| Event-based rule | An alarm is triggered if some VM-related event is generated (for example, if the MAC address of the VM conflicts with the MAC address of another VM existing in the virtual infrastructure). |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Guest volumes are running out of free disk space | An alarm is triggered if available disk space on guest volumes is below the specified threshold value. You can choose to specify the amount of due free space as an absolute value or a relative value. For example, alarm triggers if free disk space falls below 1 GB or 10% of total space. |
| Number of running services | [For Windows-based machines] An alarm is triggered if the number of services running on a VM is greater than the specified threshold. |
| Process performance | [For Windows-based machines] An alarm is triggered if the specified counter for a VM process is above or below the specified value (for example, if the CPU usage by a process exceeds 15%). |
| Process state | [For Windows-based machines] An alarm is triggered if VM process state is equal or not equal to a specific state value (Terminated, Running). |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified threshold value (for example, if the Guest Run Time level exceeds 5%). |
| Service state | [For Windows-based machines] An alarm is triggered if service state is equal or not equal to a specific state value (Running, Paused, Stopped). |
| VMs with no restore points | An alarm is triggered if the age of the latest backup or replica restore point for the VM has exceeded the threshold (that is, if there are no restore points for the specified RPO period). |
| Power or connection state changes | An alarm is triggered if the VM state reports to be equal or not equal to a specific state value (for example, if the VM is not responding). |

Cluster

Cluster

| Rule Type | Description |
| Event-based rule | An alarm will be triggered if some cluster-related event is generated. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |

Cluster Shared Volumes (CSV)

Cluster Shared Volumes (CSV)

| Rule Type | Description |
| CSV is running out of free space | An alarm is triggered if free space on the CSV is above or below the specified threshold value. You can choose to specify the free space threshold as an absolute value or a relative value. For example, an alarm is triggered if the CSV space is below 10 GB or 15% of total space. |
| Event-based rule | An alarm is triggered if some event occurs on Cluster Shared Volumes level. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Resource usage | An alarm is triggered if the specified counter is above or below the specified threshold value (for example, if read latency exceeds 40 milliseconds). |

Local Storage

Local Storage

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some storage-related event is generated. |
| Existing alarm | An alarm is triggered if the state of another selected alarm is changed. |
| Hyper-V Datastore is running out of free space | An alarm is triggered if free space on the datastore is above or below the specified threshold value. You can choose to specify the free space threshold as an absolute value or a relative value. For example, an alarm is triggered if the datastore space is below 10 GB or 15% of total space. |
| Resource usage | An alarm will be triggered if the specified counter is above or below the specified threshold value (for example, the average time of disk read exceeds 40 milliseconds). |

Any Object

Any Object

| Rule Type | Description |
| Event-based rule | An alarm is triggered if some event is generated on any object. |
| Existing alarm | An alarm is triggered if the status of another alarm specified in the settings is changed. |
| Process state | An alarm is triggered if the state of the specified process reports to be equal or not equal to a specific state value (Terminated, Running). |
| Service state | An alarm is triggered if the state of the specified service reports to be equal or not equal to a specific state value for a specified time (for example, if a service is paused for 10 minutes). |


