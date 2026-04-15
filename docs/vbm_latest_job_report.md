---
title: "Latest Job Status (Veeam Backup for Microsoft 365)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbm_latest_job_report.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Latest Job Status (Veeam Backup for Microsoft 365)


This report evaluates the success status of recently performed backup and backup copy jobs. The report shows whether they triggered any errors, warnings or completed successfully on the latest session.

* The Summary section includes the following elements:

+ The Job Statuses chart represents overall efficiency of protection operations by displaying the total number of idle jobs and jobs whose last session completed successfully/with warnings.
+ The table containing a summary of the jobs with the longest backup duration.

* The Details section displays information on all jobs performed during the reporting period: job duration and status, the number of processed objects, the amount of transferred data.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup for Microsoft 365 servers to include in the report.
* Organizations: defines Microsoft organizations to analyze in the report.
* Period: defines the time period to analyze in the report.

* Job types: defines a list of job types to evaluate in the report (Backup, Backup Copy).
* Latest job statuses: defines job session statuses to include in the report (Success, Warning, Failed).

[View Report Example](./reports/Latest%20Job%20Status%20%28Veeam%20Backup%20for%20Microsoft%20365%29.pdf)

Use Case

This report helps backup administrators track the recent Microsoft 365 object protection operations and identify root causes of failed jobs.


