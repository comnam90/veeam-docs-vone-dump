---
title: "Datastore Space Usage History"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/datastore_space_usage_history_vmware.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Datastore Space Usage History


This report analyzes the amount of space consumed by files of VMs on datastores and helps evaluate available datastore resources in the infrastructure.

* The Summary section includes the following elements:

+ The Datastores with Most Free Space and Datastores with Least Free Space charts display top datastores with the smallest and the largest amount of used space.
+ The Most Growing Datastores and Least Growing Datastores charts display top datastores with smallest and largest decrease in free space during the specified time period.

* The Details table shows datastore space usage statistics and the total number of VMs residing on datastores.

Click a datastore name to drill down to the Datastore Usage History chart that shows how the amount of free, used and provisioned space has been changing during the reporting period.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Storage type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Period: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.
* Group by: defines how data will be grouped in the report output (by Virtual Server or Datacenter).

[View Report Example](./reports/Datastore%20Space%20Usage%20History.pdf)

Use Case

The report helps you monitor storage capacities to ensure your VMs have sufficient room to operate.


