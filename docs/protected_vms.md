---
title: "Protected VMs"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/protected_vms.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Protected VMs


This report analyzes backup protection of VMware vSphere and Microsoft Hyper-V VMs in your virtual environment.

A VM is considered to be Protected if there is at least one valid backup or replica restore point that meets the designated RPO for it. A VM is considered to be Unprotected if it has an outdated or missing backup or replica restore points.

The report examines whether VMs have valid backup and replica restore points created within the specified time range (RPO period), shows the total number of restore points available for each protected VM, and provides information on the completion status of recent backup and replication job sessions.

The report helps you identify which VMs in your environment function without proper protection and make sure the existing backups and replicas meet established RPO requirements.

* The Summary section includes the following elements:

+ The Protected VMs chart shows the number of protected, unprotected VMs as well as VMs in multiple jobs (VMs in multiple jobs displays VMs that are protected by different jobs. For example, one VM with three jobs is counted as three protected VMs).
+ The VM Last Backup State chart shows status of the latest job session for discovered/protected VMs.
+ The VM Last Backup Age chart shows compliance of latest VM backups with the specified RPO requirements.

* The Details section provides information on all protected and unprotected VMs including VM location, protection type, job name, number of available restore points, date of the oldest restore point and date and time of the latest backup or replica.

|  |
| --- |
| Note: |
| * VM replicas not protected by any Veeam Backup & Replication job are not accounted in this report. * If a VM has been deleted but its restore points remain on the repository, the report will still display the VM. |

Report Parameters

You can specify the following report parameters:

* Protected infrastructure: defines the Veeam Backup & Replication infrastructure to analyze in the report.
* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VM folders: defines a list of VMware folders to include in the report (applies to VMware vSphere environments only). VM folders view is an alternate way to present the virtual infrastructure. If VMs in your infrastructure are grouped into folders according to their profile, you can limit the report scope by specifying the necessary folders only.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* RPO (Recovery Point Objective): defines the maximum amount of data that you may accept to lose, expressed in time. RPO defines the age of the latest backup or replica files required to resume normal operation if system failure occurs. For example, to compile a list of VMs protected on a daily basis, you need to set the RPO value to 1 day.
* VM exclusion rule: defines a list of VMs that should be excluded from the report scope. You can enter VM names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. For example, the following string will exclude machines with the \_R&D suffix from appearing in the report:\*\_R&D.
* Job types: defines a job type to evaluate in the report (Backup, Replication, Backup Copy, Cloud Director Backup, Cloud Director Replication, All items).
* Exclude jobs: defines a list of backup and replication jobs to exclude from the report.
* Analyze VM templates: defines whether VM templates should be included in the report.

[View Report Example](./reports/Protected%20VMs.pdf)

Use Case

When you set up your backup, replication and backup copy jobs based on VI containers (such as folders, hosts or datastores) or employ complex exclusion parameters in job properties, some VMs may turn out to be excluded from the containers and therefore will lack proper protection.

This report displays a list of VMs protected by up-to-date backups and replicas, as well as a list of unprotected VMs which have outdated or missing backup or replicas. This information helps you validate the state of backup protection in your organization.


