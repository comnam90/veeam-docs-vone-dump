---
title: "Backups on Tape"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backups_on_tape.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Backups on Tape


This report provides detailed information about backup files stored on tapes.

* The Details section provides the Details, Tape Details and Empty Tapes tables which provide information on each tape, including the amount of used space and remaining free space, size of stored backups, the date until which the tape is protected, and detailed information on backups stored on the tape.

|  |
| --- |
| Important! |
| If one restore point contains several VMs, the report will not provide detailed information on the size of individual backups for every VMs in this restore point. |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Media pools: defines a list of media pools to include in the report.
* Tapes: defines a list of tapes to include in the report.

[View Report Example](./reports/Backups%20on%20Tape.pdf)

Use Case

This report helps you monitor tape space usage and the number of VMs, computers and unstructured data files stored on tapes.


