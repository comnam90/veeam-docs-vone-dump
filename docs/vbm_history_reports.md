---
title: "Job History (Veeam Backup for Microsoft 365)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbm_history_reports.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Job History (Veeam Backup for Microsoft 365)


This report provides advanced information on completed Veeam Backup for Microsoft 365 job sessions, and helps you identify possible performance bottlenecks.

* The Summary section includes the following elements:

+ The Top 5 Jobs by Average Duration and Top 5 Jobs by Transferred Data charts display jobs in terms of the backup duration and amount of transferred data.
+ The Successful Backup Ratio by Day (%) chart displays the percentage of job sessions that completed successfully during the reporting period. If a job session finished with warning but a restore point was created successfully, the job will be displayed as successful.

* The Details table provides information on each performed job, including completion status, number of processed objects, session start time, job duration, processing rate and the amount of transferred data.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup for Microsoft 365 servers to include in the report.

* Organizations: defines Microsoft organizations to analyze in the report.

* Job types: defines a job type to evaluate in the report (Backup, Backup Copy).
* Jobs: defines a list of jobs to include in the report.
* Job status: defines a job status to include in the report (Success, Failed, Warning).
* Period: defines the time period to analyze in the report.

[View Report Example](./reports/Job%20History%20%28Veeam%20Backup%20for%20Microsoft%20365%29.pdf)

Use Case

This report shows exhaustive information on the state of recent job sessions and reveals key statistics demanded by backup operators.

You can change the default report parameters to focus on particular jobs; this will allow you to regularly receive information on vital job sessions by email or through a shared portal.


