---
title: "Veeam Backup Files Growth"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/veeam_backup_files_growth.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Veeam Backup Files Growth


This report allows you to track how the size of backup files was changing during the specified time period, and identify jobs that consume the greatest amount of space on repositories.

* The Summary section provides a general overview of repository capacity, free space, backup size and restore points as well an overview of backup jobs, job runs and stored VMs and computers. It also displays the Top 10 Jobs by Largest Backup File Size table that shows 10 jobs that produced the greatest amount of backup data during the reporting period as well as a virtual chart for each connected repository.

* The Report Data section displays Details and Extended Details tables with information on repository space usage. For each repository, the report provides a chart that illustrates the repository capacity and the amount of free space left, as well as information about restore points that were created during the reporting period, including VMs and computers in the backup, backup file type, date and time when the file was created, restore point size and total space used.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of backup repositories to analyze in the report.
* Jobs: defines a list of backup jobs to include in the report.
* Period: defines the time period to analyze in the report.

[View Report Example](./reports/Veeam%20Backup%20Files%20Growth.pdf)

Use Case

This report is useful for capacity planning purposes. The report allows you to assess historical growth of backup files and — in case backup files grow too fast — to decide whether to change job configuration to point it to another repository with larger capacity.


