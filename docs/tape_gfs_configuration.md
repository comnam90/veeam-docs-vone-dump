---
title: "Tape GFS Configuration"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/tape_gfs_configuration.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Tape GFS Configuration


The report provides information about GFS Media Pools configuration and backup to tape jobs that write restore points to the Media Pools.

* The Details section displays media pool configuration — how many tapes and tape libraries are assigned to the pool, and the number of free tapes.

* The Media Pool Configuration table provides details on media sets, such as GFS retention period for every backup restore point, how many tapes are assigned to each media set, and where tapes must be exported when a job is finished.
* The List of Tapes Assigned table shows additional information about jobs assigned to specific media sets.
* The Jobs Writings to The Media Pool section shows information about backup to tape jobs that write restore points to media pools and their backup schedule.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Media pools: defines a list of Veeam Backup & Replication GFS media pools to analyze in the report.

[View Report Example](./reports/Tape%20GFS%20Configuration.pdf)

Use Case

The report allows you to review configuration of media pools and GFS backup to tape jobs. You can trace tapes assigned to each media set, when media sets must be exported and where the exported tapes are stored.


