---
title: "Tape Media Retention Period"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/tape_media_retention_period.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Tape Media Retention Period


This report provides information on retention policy settings configured for tape media pools in Veeam Backup & Replication.

* The Summary section includes the following elements:

+ The Tapes By Expiration Status chart shows the number of protected tapes, the number of tapes with no expiration date, the number of tapes without defined expiration date and the number of tapes which can expire any time.
+ The Expired Tapes Status chart shows the share of online and offline expired tapes.

* The Report Data section information on tape media, including media pool to which the tape medium belongs, backup server, tape status, library, protection period, media set, tape, tape state, tape location, last write time, capacity (GB), free space (GB) and expiration date.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Tape status: defines whether the status of tapes to include in the report (Expired, Protected, No expiration, Other, All).

[View Report Example](./reports/Tape%20Media%20Retention%20Period.pdf)

Use Case

This report allows you to review retention policies applied to tapes and estimate available tape resources.


