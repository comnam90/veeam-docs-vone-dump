---
title: "Backup SLA Compliance (Veeam Backup for Microsoft 365)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbm_sla_reports.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Backup SLA Compliance (Veeam Backup for Microsoft 365)


This report analyzes backups of Microsoft 365 infrastructure objects. The report examines whether these objects are compliant with SLA target.

* The Summary section includes the following elements:

+ Information on SLA compliance of different organization object types.
+ The Organization Objects by Compliance State chart shows the percentage of organization objects of each type that meet the target SLA.

* The Organizations table provides information on all types of protected objects for each organization.
* The Organization Objects That Meet Target Backup SLA and Organization Objects That Breach Target Backup SLA tables provide information on all organization objects, jobs that include the objects, number of available restore points and SLA compliance percentage.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup for Microsoft 365 servers to include in the report.
* Organizations: defines Microsoft organizations to analyze in the report.
* Object types: defines Microsoft 365 infrastructure objects to analyze in the report.
* Jobs: defines backup jobs to analyze in the report.
* Period: defines the time period to analyze in the report.
* Object exclusion rule: defines a list of Microsoft 365 infrastructure objects that should be excluded from the report scope. You can enter object names either explicitly or input a part of the name. Multiple entries are separated by comma.
* Target SLA: defines the target SLA value (in percent).
* Show organization objects that missed target SLA: defines whether objects not compliant with the target SLA should be included in the report.

[View Report Example](./reports/Backup%20SLA%20Compliance%20%28Veeam%20Backup%20for%20Microsoft%20365%29.pdf)

Use Case

This report helps you discover protected objects that breach the target SLA, and jobs that do not operate properly.


