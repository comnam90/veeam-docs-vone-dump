---
title: "VM Daily Protection Status"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vm_daily_protection_status.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# VM Daily Protection Status


This report provides information on the daily backup status for all protected VMs.

The report complements the [Protected VMs](protected_vms.md) report and shows job completion results for backup, backup copy and replication tasks for protected VMs.

* The VM Backup Status chart represents overall efficiency of daily protection operations by displaying the number of VM tasks completed successfully, the number of VM tasks completed with warnings and the number of VM tasks failed. If you have launched a VM job several times a day, the report will show the best VM task status.

* The Details table provides a list of protected VMs and displays daily job completion results.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers and protected VI servers to include in the report.
* VM folders: defines a list of VMware folders to include in the report (applies to VMware vSphere environments only). VM folders is an alternate way to present the virtual infrastructure. If VMs in your infrastructure are grouped into folders according to their profile, you can limit the report scope by choosing the necessary folders only.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Interval: defines a time period to analyze in the report (Current week, Past week, Past 7 days).
* 1 week starting at: defines a time period (a week) to analyze in the report.
* 7 days starting at: defines a start date of the reporting period. The report will analyze a 7-day period starting from the selected date.
* Last <N> weeks: defines the number of weeks in the past (starting from today) to analyze in the report.
* Job types: defines a job type to evaluate in the report (Backup, Replication, Backup Copy, All).
* Analyze VM templates: defines whether VM templates should be included in the report.

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, you will not be able to generate the report based on VM folders or Business View objects. |

[View Report Example](./reports/VM%20Daily%20Protection%20Status.pdf)

Use Case

The report helps you discover issues with created backups and replicas: detect failed jobs, identify jobs that triggered warnings and ensure that critical machines can be easily recovered in case of a disaster.


