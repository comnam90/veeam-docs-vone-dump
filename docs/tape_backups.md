---
title: "Tape Backup Jobs"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/tape_backups.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Tape Backup Jobs


The main backup purpose is to protect your data against disasters and failures. Having only one copy of a backup file does not provide the necessary level of safety. To build a successful data protection and disaster recovery plan, you must have two different types of media to store copies of your data, for example, disk storage and tape.

To learn more about the 3-2-1 backup strategy, see the Veeam Blog article [How to follow the 3-2-1 backup rule with Veeam Backup & Replication](https://www.veeam.com/blog/how-to-follow-the-3-2-1-backup-rule-with-veeam-backup-replication.html).

This report maintains a record of VMs and computers archived to tapes.

* The Summary section provides information on the number of VMs and computers in backups stored on disk and archived to tapes, consumed tape capacity, and the total number of used tapes.
* The Details and Tape Details tables show properties of each backup to tape job: the total number of available restore points, restore point creation date, number of workloads in the backup file and backup type (full or incremental).

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

[View Report Example](./reports/Tape%20Backup%20Jobs.pdf)

Use Case

The report provides a summary of all backup to tape operations that took place on the managed backup server. The report displays an inventory list of items archived to the tape media. This allows you to make sure that mission critical VMs and computers have backups on tapes and are safely protected.

Page updated 2026-07-30

