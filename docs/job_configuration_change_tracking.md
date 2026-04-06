---
title: "Job Configuration Change Tracking"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/job_configuration_change_tracking.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Job Configuration Change Tracking


This report allows you to keep an eye on backup job configuration changes that occurred during a specified period.

* The Summary section includes the following elements:

+ The Job Modifications by User chart shows the number of job configuration changes performed by each authorized user.
+ The Modifications by Day chart shows the daily number of changes.

* The Details table provides information about every change performed within the reporting period, including the backup server where the change was made, the changed job, wizard page, property changed, previous and new setting values, modification date and time, and name of the user who made the change.

Report Parameters

You can specify the following report parameters:

* Scope: defines a list of Veeam Backup & Replication servers to include in the report.
* Period: defines the time period to analyze in the report.
* Users: defines users whose activity must be analyzed.
* Protection types: defines a protection type to evaluate in the report (SureBackup, VM Backup, Replication, File to tape, Backup copy, Agent backup policy, Agent backup, File backup, Â Nutanix AHV Backup and Snapshot, CDP policy, Application backup policy, Object storage backup, Object to tape backup).

[View Report Example](./reports/Job%20Configuration%20Change%20Tracking.pdf)

Use Case

Backup jobs can be configured from the Veeam Backup & Replication console, Veeam Backup Enterprise Manager console, using PowerShell scripts or through REST API. In large environments with multiple backup administrators it is often hard to tell who, when and what changed.

The report helps you review user activity, track job modifications and simplifying troubleshooting.


