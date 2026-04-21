---
title: "Custom Infrastructure"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/custom_infrastructure.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Custom Infrastructure


This report features a collection of custom properties and filters to help you analyze virtual infrastructure aspects not covered by other reports.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Object type: defines a list of infrastructure objects to analyze in the report.
* Columns: defines configuration properties to analyze in the report. The list of available properties will depend on the selected object type. Use the Filter field to search for the necessary properties by name. Note that the number of selected properties must not exceed 50.
* Custom filters: defines filters for the selected object properties.
* Group by: defines whether infrastructure objects in the report must be grouped based on the value of a specific property. To group infrastructure objects by property value, select that property from the Group by drop-down list.

You can also use the Sum, Max or Count function to calculate aggregate values of other properties for each group in the report. To do that, select the necessary aggregate functions for required properties in the list.

* Sort by: defines how data will be sorted in the report.
* Show all groups expanded: defines whether the report should display results in the collapsed or expanded view.

[View Report Example](./reports/Custom%20Infrastructure.pdf)

Use Case

Use the advanced collection of properties to report on licensing information, host hardware configuration, CPU, RAM, storage and networking performance, and many other aspects to better manage the virtual infrastructure.


