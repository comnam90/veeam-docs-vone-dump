---
title: "Alarms Overview (vSphere)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/alarms_overview_vmware.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Alarms Overview (vSphere)


Veeam ONE Client generates multiple alarms to inform you about important events in your environment. This report allows administrators to quickly review the health state of the environment and to track how the number of alarms has been changing during the reporting period.

The report analyzes alerting activity across a time range, provides information on virtual infrastructure objects that caused the greatest number of alerts, and displays top 10 most frequently occurred issues.

* The Summary section includes the following elements:

+ The Errors and Warnings charts show top 5 objects that caused the greatest number of alarms.
+ The Total Issues chart shows alarm activity during the reporting period.
+ The Top 10 Issues table shows 10 most frequently triggered alarms.

* The Details section provides information on each affected object , including object type, location, object name, number of triggered alarms and alarm activity trend.

Click a number in the Alarms column in the details table to drill down to details for alarms raised for the infrastructure object.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Business View objects: defines Business View groups to analyze in the report.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Period: defines the time period to analyze in the report. Note that the reporting period must include at least one successfully completed Object properties data collection task for the selected scope. Otherwise, the report will contain no data.
* Group by: defines how data will be grouped in the report output (by Issue type or Object type).
* Object types: defines a list of virtual infrastructure object types to analyze in the report.
* Alarms: defines a list of alarms to analyze in the report.

For details on alarms you can select in the list, see [VMware vSphere Alarms](vsphere_alarms.md).

[View Report Example](./reports/Alarms%20Overview%20%28vSphere%29.pdf)

Use Case

The report provides an overview of the current health state of your virtual environment, shows the list of the most common alarms and identifies the most affected virtual infrastructure objects.


