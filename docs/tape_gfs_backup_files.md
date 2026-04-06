---
title: "Tape GFS Backup Files"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/tape_gfs_backup_files.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Tape GFS Backup Files


This report provides historical information about backups for Veeam Backup & Replication backup to tape with GFS retention policy.

* The Summary section provides information on the number of GFS media pools, number of historical backup files, number of restore points in these files, and the amount of space consumed by historical backup files on tape.

+ The Historical Restore Points Count chart shows the number of daily, weekly, monthly, quarterly and yearly restore points in historical backup files.

* The Details table provides information about historical restore points in GFS media pools, including the media set, number of VMs and computers, date when restore point was created, name of a tape job that created the restore point, and ID of tapes on which the restore point resides.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Media pools: defines a list of Veeam Backup & Replication GFS media pools to analyze in the report.

[View Report Example](./reports/Tape%20GFS%20Backup%20Files.pdf)

Use Case

The report allows you to inventory historical backups on tape created in accordance with the GFS retention scheme. You can track historical restore points on tape and make sure that you have backups archived for long-term retention.


