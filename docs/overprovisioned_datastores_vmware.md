---
title: "Over-Provisioned Datastores (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/overprovisioned_datastores_vmware.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Over-Provisioned Datastores (vSphere)


Thin provisioning allows administrators to dedicate more datastore space to VMs than there is real physical capacity. This report helps you assess the potential impact of excessive over-provisioning of datastores on performance of your virtual environment.

* The Summary section includes the following elements:

+ The TOP 5 Over-provisioned Datastores chart shows 5 datastores whose amount of provisioned storage space exceeds the total capacity.
+ The TOP 5 Under-provisioned Datastores chart shows 5 datastores whose amount of provisioned storage space is way below the total capacity.
+ The TOP 5 Datastores with Least Amount of Free Space table displays top 5 datastores that will run out of free space sooner than other datastores.

Click a number in the VM Count column to get the list of VMs that store data on the datastore and to discover how much space is provisioned for these VMs.

* The Details section provides information on storage space utilization and the number of days left before the specified space utilization/free space threshold will be breached. Arrows in the Out of Free Space in … (Days) column show whether the amount of free space on the datastore has increased (green arrow), decreased (red arrow) or stayed the same (grey arrow) over the previous week.

Click a number in the VM Count column to get the list of VMs that store data on the datastore and to discover how much space is provisioned for these VMs.

Click a number in the Out of Free Space in … (Days) column to drill down to performance details for the datastore.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Storage type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Space utilization threshold: defines the threshold for the amount of space in use on datastores.
* Minimum free space threshold: defines the threshold for the amount of free space left on datastores.
* Show graphs: defines whether to include charts in the report output.

[View Report Example](./reports/Over-Provisioned%20Datastores%20%28vSphere%29.pdf)

Use Case

The report analyzes datastore space utilization trend and calculates the number of days left before storage utilization will breach the specified threshold.


