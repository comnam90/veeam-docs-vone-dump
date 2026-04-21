---
title: "CDP SLA Compliance"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/cdp_sla_compliance.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# CDP SLA Compliance


This report analyzes continuous data protection of VMs in your virtual infrastructure. The report examines whether VMs protected by CDP policy are compliant with SLA target.

* The Summary section includes the following elements:

+ The Average SLA chart shows the average SLA percentage for protected and unprotected VMs.
+ The Workloads by Compliance State chart shows the number of VMs that meet the target SLA, VMs that breach the target SLA and VMs that do not have a CDP replica.
+ The Workloads by SLA chart shows the SLA value for protected and unprotected VMs.
+ The Sync Sessions Statistics chart shows number of job sessions for protected and unprotected VMs finished with different statuses.

* The Report Data section displays three tables, Workloads That Meet Target SLA, Workloads That Missed Target SLA, and CDP Sessions Issues and provides information on all VMs protected by CDP policies, including VM name, CDP policy name, VM location, replica location, RPO, average SLA, maximum delay, number of crash-consistent and application-consistent restore points, status of the last replication session, amount of transferred data, primary bottleneck and date and time of the last successful replication session.

Report Parameters

You can specify the following report parameters:

* Protected infrastructure: defines the platform to analyze in the report.

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.

* VM folders: defines a list of VMware folders to include in the report (applies to VMware vSphere environments only). VM folders view is an alternate way to present the virtual infrastructure. If VMs in your infrastructure are grouped into folders according to their profile, you can limit the report scope by specifying the necessary folders only.

* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.
* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.

* Period: defines the time period to analyze in the report.
* VM exclusion rule: defines a list of VMs that should be excluded from the report scope. You can enter VM names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by comma. Usage example: the following string will exclude machines with the \_R&D suffix from appearing in the report:\*\_R&D.
* Target SLA: defines the target SLA value (in percent).
* Show non-compliant VMs: defines whether VMs not compliant with the target SLA should be included in the report. You can choose to show all non-compliant VMs or only VMs added to CDP policies.
* Include Business View groups: defines whether to include business view groups in the report.

[View Report Example](./reports/CDP%20SLA%20Compliance.pdf)

Use Case

This report helps you discover VMs that breach the target SLA or do not have a CDP replica. It provides details on the state of CDP policies so that you can reconfigure current policy settings or include mission critical VMs in CDP policies.


