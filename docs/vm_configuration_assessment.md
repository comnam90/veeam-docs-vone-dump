---
title: "VM Configuration Assessment"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vm_configuration_assessment.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# VM Configuration Assessment


This report helps you to assess VMs readiness for performing backup with Veeam Backup & Replication. The report analyzes configuration of VMs in your virtual environment, and shows potential issues and possible limitations that could cause backup process to fail or prevent VMs from being properly backed up.

* The Summary section contains the following charts:

+ The Virtual Machines Overview chart shows VMs with potential issues and ready to backup VMs.
+ The Potential Issues chart shows number of VMs with potential issues.

* The Details section provides information on VMs with potential issues and recommendations on resolving the issues.

The report takes into account the following criteria when analyzing VM configuration:

VMware CBT

VMware CBT

| Criterion | Description |
| Existing Snapshots | The report analyzes your virtual infrastructure to find VMs with existing snapshots.  To use VMware Changed Block Tracking for incremental backup, all existing snapshots must be removed. |
| Hardware Version 4 or earlier | The report analyzes your virtual infrastructure to find VMs with hardware version 4 or earlier.  To use VMware Changed Block Tracking for incremental backup, hardware version of VMs must be 7 or later. |

Virtual Disks

Virtual Disks

| Criterion | Description |
| VMs with Independent Disks | The report analyzes your virtual infrastructure to find VMs with independent virtual disks.  Veeam Backup & Replication does not support independent disks; these disks are skipped from processing automatically. |
| VMs with 2 TB virtual disks running in vSphere 5.1 or older | The report analyzes your virtual infrastructure to find VMs with 2 TB virtual disk size.  For ESXi 5.1 and older, the maximum virtual disk (VMDK) size for snapshot operations is limited to 1.9844923662017202 TB. For details on, see [this VMware KB article](https://kb.vmware.com/s/article/2058287). |
| VMs with disks engaged in SCSI bus sharing | The report analyzes your virtual infrastructure to find VMs that use SCSI bus-sharing.  VMware does not support taking snapshots of Microsoft Clustering Services (MSCS) VMs. For details on, see [this VMware KB article](https://knowledge.broadcom.com/external/article/311074/unable-to-use-snapshots-or-perform-a-bac.html). |
| Virtual disk size is not a multiple of 1 KB | The report analyzes your virtual infrastructure to find VMs with unaligned virtual disks.  Veeam Backup & Replication does not support backup copy jobs and restore jobs for VMs with unaligned disks. For details on, see [this Veeam KB article](https://www.veeam.com/kb1848). |
| VMs with pRDMs | The report analyzes your virtual infrastructure to find VMs with RDMs used in physical compatibility mode.  Veeam Backup & Replication will automatically exclude RDMs used in physical compatibility mode from the backup job. For details on, see [this VMware KB article](https://kb.vmware.com/s/article/2009226). |

Application-Aware Image Processing

Application-Aware Image Processing

| Criterion | Description |
| VMs with Windows Server 2000 Guest OS | The report analyzes your virtual infrastructure to find Windows Server 2000 VMs.  To enable backup with application-aware image processing, upgrade guest OS to Windows Server 2003 or later. |
| VMware Tools Not Running | The report analyzes your virtual infrastructure to find VMs that do not have with VMware Tools installed or running.  To enable backup with application-aware image processing, it is required that guest OS running inside your VMs has VMware Tools installed and running. |

Datastore Free Space

Datastore Free Space

| Criterion | Description |
| VMs on datastores with 10% of free space | The report analyzes your virtual infrastructure to find datastores that have less than 10% of free space.  When Veeam Backup & Replication backs up a VM, it triggers a VMware snapshot that is normally stored next to VM files on the source datastore. To eliminate the problem of datastores running low on free space during backup, it is required that the free space is more than 10%. |

Other

Other

| Criterion | Description |
| Unsupported VM names | The report analyzes your virtual infrastructure to find VMs with names that contain the following symbols: @ / \ < >.  Veeam Backup & Replication does not process VMs with names that contain mentioned symbols. If you want to back up these virtual machines, you must rename them. |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Issues: defines VM assessment criteria to include in the report.
* Ignore replica VMs created by Veeam products: defines whether to include in the report VM replicas created with Veeam Backup & Replication.

[View Report Example](./reports/VM%20Configuration%20Assessment.pdf)

Use Case

This report allows you to obtain a list of VMs in your virtual environment that could experience potential issues with backups, and to get guidance on how to resolve these issues.


