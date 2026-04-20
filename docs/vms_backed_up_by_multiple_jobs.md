---
title: "VMs Backed Up by Multiple Jobs"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vms_backed_up_by_multiple_jobs.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# VMs Backed Up by Multiple Jobs


This report analyzes configuration of backup jobs to find VMs that are simultaneously included in several jobs. This helps you reduce backup windows and optimize backup infrastructure operation.

* The Summary display includes the following elements:

+ The VMs with Largest Avg. Transferred Data (GB) chart shows top 5 VMs with the largest amount of transferred backup data.
+ The VMs with Largest Processing Time (Minutes) chart shows top 5 VMs with the longest time interval required to produce a VM backup.

* The Report Data table provides information on the list of backup servers, backup jobs in which the VM is included, job schedules, target repository names, the average processing time, average VM transferred data (in GB), the number of restore points created for the VM, full backups and the last time the jobs ran.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Exclude jobs: defines a list of backup and replication jobs to exclude from the report.

[View Report Example](./reports/VMs%20Backed%20Up%20by%20Multiple%20Jobs.pdf)

Use Case

The reason why some VMs may appear to be backed up by several jobs at a time can be a lack of coordination between several backup operators or the capability to include logical containers (vApps, resource pools, folders) in backup jobs. Both issues can cause repositories to run out of free space due to excessive duplicated backup files.

The report allows you to assess efficiency of the backup process and decide whether to reconfigure existing backup jobs so that they utilize fewer resources and complete in narrower intervals. This report ensures that all critical VMs are reliably protected while no redundant jobs exist across the backup environment.


