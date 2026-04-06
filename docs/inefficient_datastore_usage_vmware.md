---
title: "Inefficient Datastore Usage"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/inefficient_datastore_usage_vmware.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Inefficient Datastore Usage


This report provides an overview of storage devices that accommodate inactive virtual machines.

* The Storage Consumed by Inactive VMs (GB) chart displays the amount of storage space consumed by VMs that have been inactive for one month, six months and one week.
* The Details table shows the full list of inactive VMs and rates the VMs by the amount of consumed storage.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.

* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

[View Report Example](./reports/Inefficient%20Datastore%20Usage.pdf)

Use Case

Inactive VMs consume valuable storage space. Use this report to review performance of your VMs and identify VMs that can be deleted or relocated to less costly datastores to reclaim additional storage space.


