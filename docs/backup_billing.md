---
title: "Backup Billing"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/backup_billing.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Backup Billing


This report allows you to assess storage costs for the backup infrastructure and to track the consumption of storage by backup files.

The report estimates storage resources required to store backups. The cost can be calculated based on the price of 1 GB or TB of consumed storage space or on the price of a single VM. If there is a repository that is more expensive than other ones, an administrator can also specify the price adjustment factor (or the multiplier) that characterizes the premium charged for access to the repository.

The report provides details on every backup job included into the report scope — the number of backed up VMs and computers, size of a restore point and total amount of gigabytes transferred to the storage.

* The Summary section provides an overview on the number of backup jobs, used repositories and backed up VMs and computers, total size of backups and total cost in selected currency.
* The Details section provides information on each backup job, including the number of backed up VMs and computers, restore points size, total amount of gigabytes transferred to the storage and total cost.

|  |
| --- |
| Important! |
| If one restore point contains several VMs, the report will not provide detailed information on the size of individual backups for every VMs in this restore point. For details on, see [Backup Chain Formats](https://helpcenter.veeam.com/docs/backup/vsphere/per_vm_backup_files.html). |

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of backup repositories to analyze in the report.

* Business View objects: defines a list of Business View objects to analyze in the report.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Job type: defines a job type to evaluate in the report (VM backup, Backup copy, Agent backup policy, Agent backup, All types).
* Jobs: defines a list of backup and backup copy jobs to include in the report.

* Period: defines the interval for which the billing statement is required.
* Storage price: defines a storage price for accommodating 1 GB/TB of backup files or a price for a single VM included in backup.

* Individual repository price multipliers: defines the price adjustment factor that characterizes the benefit (and the expense) of using the preferred repository storage. The resulting cost is calculated by multiplying the basic rate by the repository multiplier.

To edit price multipliers:

1. Click Configure.
2. In the Configure Individual Repository Price Multipliers window, select the target repository and click Edit.
3. In the Set Individual Repository Price Multiplier window, specify the desired price adjustment multiplier and click Save.
4. For scale-out backup repositories:

* To include capacity and archive tiers in the list of extents, select the Count data stored on Capacity and Archive tier extents check box.

* To set a single multiplier for all extents of a scale-out backup repository, select the Specify the same multiplier for each extent check box and specify the multiplier.

* To apply an individual multiplier to each extent, click the value in the Multiplier column next to an extent and specify the multiplier.

1. Repeat steps 2–3 for each repository price multiplier you want to edit.

* Calculate price based on: defines the value based on which prices will be calculated (Latest value, Max value).
* Customer: defines a customer name to display in the report output.
* Show days with no backup activities: defines whether the report will include days without backup activity.

[View Report Example](./reports/Backup%20Billing.pdf)

Use Case

This report allows managed storage providers (MSP) to generate billing statements for customers and to charge them for the used storage.

The report can help administrators evaluate efficiency of the storage resources utilization.


