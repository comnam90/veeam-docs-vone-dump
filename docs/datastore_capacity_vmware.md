---
title: "Datastore Capacity"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/datastore_capacity_vmware.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Datastore Capacity


This report helps administrators evaluate available datastore capacities across the infrastructure.

* The Storage Overview (Top N) chart shows top datastores with the greatest amount of used disk space.

Click the Details link at the bottom of the chart to drill down to the list of datastores that includes details on total storage capacity, the amount of free and used space, and the number of VMs that reside on these datastores.

* The Virtual Disks Capacity (Top N) chart shows top VMs with the greatest virtual disk size.

Click the Details link at the bottom of the chart to drill down to the full list of VMs that includes details on total virtual disk size, snapshot size, and the power state of these VMs.

* The Logical Disks (Top N) chart shows top VMs with greatest logical disk size.

Click the Details link at the bottom of the chart to drill down to the full list of VMs that includes details on total logical disk capacity, the amount of free and used space, and the power state of these VMs.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Storage type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Top N: defines the number of top datastores, virtual and logical disks that will be displayed in the report charts.

[View Report Example](./reports/Datastore%20Capacity.pdf)

Use Case

The report helps you monitor storage capacities to ensure your VMs have sufficient room to operate.


