---
title: "Datastore Configuration (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/datastore_configuration_vmware.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Datastore Configuration (vSphere)


This report documents the current configuration of datastores in your infrastructure.

* The Summary section includes the following elements:

+ The Utilization (%) chart shows the amount of free and used space on datastores.
+ The Provisioned Space (GB) chart shows datastores capacity and the amount of space provisioned to VMs.
+ The summary table provides configuration details for each datastore, including the datastore capacity, amount of free space, amount of provisioned space, provisioning ratio (datastore capacity against provisioned space) and free space usage trend.

Click a hyperlink in the Free Space Usage Trend column table to drill down to daily information on total capacity, the amount of used and provisioned space, and the number of VMs residing on the datastore.

* The Top 3 VMs section shows VMs that consume more storage space than other VMs.
* The General Information table provides information about the datastore owner, datastore type, file system, block size, and the number of VMs residing on the datastore.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Storage type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

[View Report Example](./reports/Datastore%20Configuration%20%28vSphere%29.pdf)

Use Case

The report helps you monitor storage capacities to ensure your VMs have sufficient room to operate.


