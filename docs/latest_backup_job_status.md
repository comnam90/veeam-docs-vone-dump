---
title: "Latest Job Status"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/latest_backup_job_status.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Latest Job Status


This report evaluates the success status of recently performed backup, replication and backup copy jobs. The report shows whether they triggered any errors, warnings or completed successfully on the latest session.

* The Summary display includes the following elements:

+ The Job Status chart represents overall efficiency of workload protection operations by displaying the total number of idle jobs and jobs whose last session completed successfully/with warnings.
+ The Top 10 Jobs by Duration table provides a summary of the top 10 jobs with the longest backup duration.

* The Report Data display shows two tables.

* The Details table shows information on backup servers, all jobs performed during the reporting period: job duration, last run and status, objects in job, backed up objects in job, objects with anomalies, the number of processed workloads, the amount of transferred data, retry count, average duration and duration trends. For failed jobs, the report also shows error text.
* The Additional Details table shows information additionally to the details table including object names, backup types, transferred data (in GB), job details, vApp names and object types.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Period: defines the time period to analyze in the report.

* Job types: defines a list of job types to evaluate in the report (VM backup, Replication, File to tape, Backup to tape, Backup copy, Agent backup policy, Agent backup, Cloud Director Backup, Cloud Director Replication and Object Storage job types).
* Latest statuses: defines a job run status to include in the report (Success, Warning, Failed).

[View Report Example](./reports/Latest%20Job%20Status.pdf)

Use Case

This report helps backup administrators track the recent VM protection operations and identify root causes of failed jobs.


