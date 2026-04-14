---
title: "Orphaned VMs"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/orphaned_vms.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Orphaned VMs


This report discovers VMs that are present in existing backup files, but are missing in backup, replication or backup to tape jobs. The report examines the content of backups on disk and tape and compares this data to the configuration properties of scheduled jobs, listing VMs that are not included in the jobs.

* The Summary section includes the VMs without Backup Jobs chart that shows the number of VMs that are not included in jobs.

* The Details table provides information on orphaned VMs, including protection type, the number of restore points, backup location, the date of the last backup session and the date when the backup will be deleted according to the current file retention policy.

Report Parameters

You can specify the following report parameters:

* Scope: defines a list of Veeam Backup & Replication servers to include in the report.
* Protection type: defines a job type to include in the report (Backup, Replication, Archive, All).

[View Report Example](./reports/Orphaned%20VMs.pdf)

Use Case

A VM may become orphaned due to an error or oversight, job misconfiguration or a lack of coordination between several backup administrators, for example, when someone changed the configuration of the job and by mistake forgot to include the VM in that job. A VM may also become orphaned due to some automatic procedures, for example, when the VM migrated to an unprotected host through vMotion or as a result of DRS activating.

This report helps decide whether to modify the backup job settings for the VM if it is a mission critical one, or to delete the VM from the backup if it is no longer necessary.


