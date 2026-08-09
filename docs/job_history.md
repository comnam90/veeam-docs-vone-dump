---
title: "Job History"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/job_history.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Job History


This report provides advanced information on completed backup and replication job sessions, and helps you identify possible performance bottlenecks.

* The Summary display includes the following elements:

* The Top 5 Jobs by Average Duration and Top 5 Jobs by Transferred Data charts display top 5 jobs in terms of the longest backup duration and the largest amount of transferred data.
* The Successful Backup Ratio by Day (%) chart displays the percentage of backup and replication job sessions that completed successfully during the reporting period. If a job session finished with warning but a restore point was created successfully, the job will be displayed as successful.

* The Report Data display includes the following elements:

* The Job Details table displays a log of all backup and replication job sessions, including key metrics such as job duration, data size, and transfer rate. Use this table to review historical job performance.
* The Job Details (Unstructured Data) table displays job history details for file share and object storage backups, focusing on jobs that protect unstructured data sources.
* The VM Details table displays per-object details for a specific backup job run, listing each processed virtual machine and showing individual performance metrics such as processing speed and resource usage.
* The Unstructured Data Details table displays a per-source breakdown for an unstructured data backup job, listing each file share or object storage source with associated metrics.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Job type: defines a job type to evaluate in the report (Backup to tape, Cloud backup policy, Cloud Director backup, Cloud Director replication, File to tape, Nutanix backup, Object to tape backup, Replication, Unstructured data backup, Unstructured data copy, VM backup, VM copy).
* Jobs: defines a list of backup and replication jobs to include in the report.
* Job status: defines a job status to include in the report (Success, Success and warnings, Failures and warnings, Failures only, All).
* Period: defines the time period to analyze in the report.

[View Report Example](./reports/Job%20History.pdf)

Use Case

This report shows exhaustive information on the state of recent job sessions and reveals key statistics demanded by backup operators.

You can change the default report parameters to focus on particular jobs that include critical VMs; this will allow you to regularly receive information on vital job sessions by email or through a shared portal.

Page updated 2026-08-06

