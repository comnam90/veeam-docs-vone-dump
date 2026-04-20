---
title: "Protected VMs (Nutanix AHV)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/protected_nutanix_vms.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Protected VMs (Nutanix AHV)


This report analyzes backup protection of Nutanix AHV VMs in your backup environment.

A VM is considered to be Protected if there is at least one valid backup restore point that meets the designated RPO for it. A VM is considered to be Unprotected if it has an outdated or missing backup restore points.

* The Summary section includes the following elements:

+ The Protected VMs chart shows the number of protected and unprotected VMs.
+ The Last Backup State chart shows status of the latest job session for discovered/protected VMs.
+ The Unprotection Reason chart shows reasons for non-compliance with the specified RPO requirements.

* The Details section provides information on all protected and unprotected VMs including name of a Nutanix AHV cluster, protection domain to which the VM is added, job name, backup target, number of available restore points and date and time of the latest backup.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* RPO (Recovery Point Objective): defines the maximum amount of data that you may accept to lose, expressed in time. RPO defines the age of the latest backup files required to resume normal operation if system failure occurs. For example, to compile a list of VMs protected on a daily basis, you need to set the RPO value to 1 day.
* VM exclusion rule: defines a list of VMs that should be excluded from the report scope. You can enter VM names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. Usage example: the following string will exclude machines with the \_R&D suffix from appearing in the report:\*\_R&D.
* Backup jobs: defines a list of backup jobs to evaluate in the report.

[View Report Example](./reports/Protected%20VMs%20%28Nutanix%20AHV%29.pdf)

Use Case

When you set up your backup jobs based on protection domains or employ complex exclusion parameters in job properties, some VMs may turn out to be excluded from the protection domains and therefore will lack proper protection.

This report displays a list of VMs protected by up-to-date backups, as well as a list of unprotected VMs which have outdated or missing backup. This information helps you validate the state of backup protection in your organization.


