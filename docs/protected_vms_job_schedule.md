---
title: "Protected VMs Job Schedule"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/protected_vms_job_schedule.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Protected VMs Job Schedule


This report publishes the timetable for all scheduled backup, replication and backup copy jobs. The report analyzes all recurrent jobs in the selected scope and reveals advanced details:

* The Summary section includes the following elements:

+ The Jobs Schedule chart displays the total number of jobs running according to the specified schedules.
+ The Protected VMs chart displays the total number of VMs protected by scheduled backup, replication and backup copy jobs.

* The Details table shows VMs included in the jobs, scheduled run time and date, recurrence intervals, weekly full backup schedule for backup jobs and the effective backup file retention policy.

Report Parameters

You can specify the following report parameters:

* Protected infrastructure: defines the platform to analyze in the report.

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Job types: defines a job type to evaluate in the report (VM backup, Replication, Backup copy).
* VM exclusion rule: defines a list of VMs that should be excluded from the report scope. You can enter VM names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. Usage example: the following string will exclude machines with the \_R&D suffix from appearing in the report:\*\_R&D.
* Analyze VM templates: defines whether VM templates should be included in the report.

[View Report Example](./reports/Protected%20VMs%20Job%20Schedule.pdf)

Use Case

This report helps you ensure that applied data protection job schedules are configured in accordance to the backup policies and allow you to meet the desired RPO requirements.


