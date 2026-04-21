---
title: "Computer Backup Status"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/computer_backup_status.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Computer Backup Status


This report provides information on daily backup status for all protected and unprotected computers.

* The Summary display contains the Agents Backup Status chart that displays the number of jobs whose sessions completed successfully, the number of jobs whose sessions completed with warnings and the number of jobs whose sessions failed. If a job has been launched several times a day, the report shows the best job status. If a job includes multiple computers, each computer has its own status in the chart and the report shows the best result of the job for each agent.
* The Report Data display provides a list of protected agents and displays daily job completion results.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Computer type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Backup jobs/policies: defines a list of agent backup jobs to include in the report.
* Agent types: defines types of Veeam backup agents to include in the report.
* Period: defines a time period to analyze in the report (number of weeks from 1 to 10).
* Computer inclusion rule: defines names of computers to include in the report.

[View Report Example](./reports/Computer%20Backup%20Status.pdf)

Use Case

The report helps you detect failed agent backup jobs, identify jobs that triggered warnings and ensure that protected computers can be easily recovered in case of a disaster.


