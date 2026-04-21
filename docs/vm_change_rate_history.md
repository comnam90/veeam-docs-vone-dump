---
title: "Data Change Rate History"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vm_change_rate_history.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Data Change Rate History


This report allows you to track backup and replication jobs and workloads whose backup files and replicas grow too fast and may quickly consume storage space on the target repository or target datastore.

* The Change Rate History chart shows percentage of VMs and computers data changes that took place during the reporting period.
* The Objects with Largest Change Rate (GB) and Objects with Least Change Rate (GB) charts displays the most and least active VMs and computers in terms of the amount of data changes that occurred on their virtual disks.

* The Details table provides information on the list of workloads included in the backup and replication jobs, the average and aggregate amount of data changes that took place during the reporting period, the number of full backups and increments, and the size of the current full backup file\*.

Click a VM name to drill down to change rate statistics for each day of the reporting period.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VM folders: defines a list of VMware folders to include in the report (applies to VMware vSphere environments only). VM folders is an alternate way to present the virtual infrastructure. If VMs in your infrastructure are grouped into folders according to their profile, you can limit the report scope by specifying the necessary folders only.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Backup Infrastructure objects: defines Veeam Backup & Replication servers to analyze in the report.
* Period: defines the time period to analyze in the report.
* Job types: defines a job type to evaluate in the report (VM Backup, Replication, Agent backup policy, Agent backup, All items).
* Exclude jobs: defines a list of backup and replication jobs to exclude from the report.
* Calculate change rate based on: defines the way change rate will be calculated in the report (based on Data transferred or Data read).

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client may show invalid data for Veeam Backup & Replication reports and dashboards. |

[View Report Example](./reports/Data%20Change%20Rate%20History.pdf)

Use Case

To perform incremental backup, Veeam Backup & Replication needs to know which data blocks have changed since the previous job run. For VMware VMs with hardware version 7 or later, Veeam Backup & Replication employs VMware vSphere Changed Block Tracking (CBT) — a native VMware feature that backs up only the list of VM blocks that have changed since the last run of this particular job. Use of CBT reduces backup session duration, and increases the speed and efficiency of block‑level incremental backups.

The report analyzes changes occurred on VM disks and estimates the amount of changed data. This can help you decide whether to allocate more space on the target repository or datastore in case VM files grow too fast.

The report is also handy for people planning to do replication as a way to figure out if their bandwidth can handle the replication.

\*Note that no data will be available for synthetic or reversed backup, as well as for replicas.


