---
title: "Licensed Objects"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/licensed_objects.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Licensed Objects


Veeam ONE can be licensed in two ways: per-socket and per-instance.

Per Socket Licensing

Veeam ONE can be licensed by the number of CPU sockets on managed VMware vSphere and Microsoft Hyper-V hosts. A license is required for every occupied motherboard socket as reported by the hypervisor API. A managed host is a host that is included in the monitoring and reporting scope with Veeam ONE inclusion rules. For details, see [Choosing VMs and VM Containers to Monitor and Report On](vms_to_monitor.md).

Per Instance Licensing

Veeam ONE can be licensed by the number of instances. An instance is a unit (or token) that is assigned to an object to make it manageable in Veeam ONE.

Veeam ONE per-instance license apply to the following types of objects:

* VMs protected by the monitored Veeam Backup & Replication servers and VMs included in the monitoring and reporting scope with Veeam ONE inclusion rules. For details on configuring monitoring scope for the virtual infrastructure, see [Choosing VMs and VM Containers to Monitor and Report On](vms_to_monitor.md).

VMs protected by the monitored Veeam Backup & Replication servers and VMs included in the monitoring and reporting scope at the same time consume one instance from a license scope. Powered off replicas do not consume instances.

* Computers protected with Veeam Agent for Windows, Linux, Mac, IBM AIX and Oracle Solaris that are managed by Veeam Backup & Replication servers that you connect to Veeam ONE.

The number of instances consumed by a managed computer depends on the mode in which the Veeam Agent job operates. For details on Veeam Agent licensing coefficients, see section Instance calculation for Veeam Universal License of the [Veeam Licensing Policy](https://www.veeam.com/licensing-policy.html).

* File shares protected by Veeam Backup & Replication servers that you connect to Veeam ONE. File shares are licensed per 500 GB of protected data.
* Nutanix AHV, oVirt Kernel-based and Proxmox VMs protected by Veeam Backup & Replication servers that you connect to Veeam ONE.
* Cloud VMs, cloud databases and cloud file shares protected by Veeam Backup for Microsoft Azure, Veeam Backup for AWS and Veeam Backup for Google Cloud integrated with Veeam Backup & Replication servers that you connect to Veeam ONE.
* Microsoft 365 user accounts whose data is protected with Veeam Backup for Microsoft 365 servers connected to Veeam ONE.

|  |
| --- |
| Note: |
| * Rental program for Veeam Cloud & Service Providers (VCSP) includes free license usage for Veeam Backup for Microsoft 365 monitoring. Consider that when you generate the license, Microsoft 365 (10 users pack) costs 2 PPU. When you submit your monthly license usage report, the cost of the license will be changed to 0 PPU. * If you have full monitoring enabled with your licenses for Veeam ONE and Veeam Backup for Microsoft 365, monitoring of Veeam Backup for Microsoft 365 does not consume any license units. |

* Enterprise Applications protected with Veeam Plug-ins for SAP HANA, Oracle RMAN, SAP on Oracle, Microsoft SQL Server, SAP MaxDB.
* Object Storage data protected by Veeam Backup & Replication servers that you connect to Veeam ONE. Object storage protection is licensed per 500 GB of protected data.

Rental licenses intended for Veeam Cloud & Service Providers (VCSP) use points as license units. For details on rental licenses, see [Veeam ONE](https://helpcenter.veeam.com/docs/vcsp/refguide/veeam_one.html).

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise license instances may be consumed incorrectly. |

New Objects

To provide more flexibility and introduce a trial period for object management, Veeam ONE offers the concept of New objects for Rental licenses. New objects are objects that were discovered within the current calendar month. New objects are tracked separately. The Used points license counter reflects the number of points required for the new objects, that is the number of new objects multiplied by the object coefficient.

New objects do not consume the license points until the beginning of the new month. On the first day of the new month, the number of new objects is added to the number of managed objects and the New points counter in the license resets. New objects are not included in a license usage report.

|  |
| --- |
| Note: |
| The New objects counter in Veeam ONE does not include:   * File shares protected by Veeam Backup & Replication * Nutanix VMs, Microsoft Azure VMs and AWS EC2 instances that are not included in the New objects counter on the monitored Veeam Backup & Replication server |

Page updated 2026-07-15

