---
title: "VMs Growth (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vms_growth_vmware.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# VMs Growth (vSphere)


This report tracks how the number of VMs in your virtual environment has been changing during the reporting period. The report analyzes the amount of allocated resources, displays changes in the number of VMs, and shows how these changes influenced resource provisioning in the infrastructure.

* The Summary section provides information on the total number of VMs, number of added and removed VMs, allocated vCPU, memory and storage resources, allocation ratios and VMs growth during the reporting period.
* The Added VMs Details table provides information on each added VM, including VM location, name, number of vCPUs, allocated memory and storage resources, initiator and the date and time when the VM was added.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Period: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.

[View Report Example](./reports/VMs%20Growth%20%28vSphere%29.pdf)

Use Case

This report allows you to control virtual machine sprawl and to optimize resource utilization in your infrastructure.


