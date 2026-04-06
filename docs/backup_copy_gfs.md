---
title: "GFS Backup Files"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_copy_gfs.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# GFS Backup Files


This report provides historical information about restore points for Veeam Backup & Replication jobs with the Grandfather-Father-Son (GFS) retention policy.

* The Summary section provides information about jobs configured with the GFS retention policy, the number of historical backup files, restore points in these files and the amount of space occupied by historical backup files.

+ The Restore Points Age chart shows the share of weekly, monthly and yearly restore points.
+ The Top 5 Jobs by Number of Restore Points chart displays 5 jobs with the greatest number of GFS restore points.

* The Next Restore Points to Be Deleted by Retention table shows restore points that will soon be deleted according to the retention policy, as well as their size, type and objects they contain.

Click a job name to drill down to the job details section.

* The Job subsections display information about jobs with GFS retention policy: job retention configuration, a list of existing restore points and their details. You can also view distribution of GFS restore points of all types for the current calendar year.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Job types: defines a job type to evaluate in the report (VM backup, Backup copy, Agent backup, Agent backup policy, All items).
* Jobs: defines a list of jobs to analyze in the report.

[View Report Example](./reports/GFS%20Backup%20Files.pdf)

Use Case

If you have a large backup infrastructure with a great number of restore points with GFS retention policy, you may find it difficult to track these points. The report allows you to inventory restore points created with the GFS retention policy, and check what restore points will soon be removed by retention.


