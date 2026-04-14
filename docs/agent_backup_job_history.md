---
title: "Agent Backup Job and Policy History"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/agent_backup_job_history.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Agent Backup Job and Policy History


This report provides historical information for Veeam agent backup policies and job sessions results.

* The Summary display includes the following elements:

+ The Top 5 Jobs and Policies by Restore Points Created and Top 5 Jobs and Policies by Backed up Data charts display top 5 jobs and policies in terms of the greatest number of restore points and the largest amount of backed up data.
+ The Agent Backup Jobs and Policies Result chart shows the number of jobs and policies whose sessions completed successfully, the number of jobs and policies whose sessions completed with warnings and the number of jobs and policies whose sessions failed.

* The Jobs and Policy - Overview table provides information on each performed agent backup job: session date, number of backed up agents and created restore points, the completion state and total backup size.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Backup jobs/policies: defines a list of backup jobs and policies to include in the report.
* Period: defines the time period to analyze in the report.

[View Report Example](./reports/Agent%20Backup%20Job%20and%20Policy%20History.pdf)

Use Case

This report allows you to track historical statistics, amount of backed up data and created restore points for all agent backup jobs and policies.


