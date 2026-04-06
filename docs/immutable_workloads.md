---
title: "Immutable Workloads"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/immutable_workloads.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Immutable Workloads


This report lists workloads and their restore points providing information on whether immutability targets are met by these workloads and their backups.

* The Summary section provides the numbers of mutable and immutable workloads and restore points as well as their immutability ratio, and includes the following elements:

+ The Workloads by Immutability chart shows the number of mutable and immutable workloads.
+ The Restore Points by Immutability chart shows the number of mutable and immutable restore points.
+ The Workload Types by Immutability chart shows the number of mutable and immutable workloads of each workload type.

* The Details table provides information about every immutable and mutable workload including the workload platform, name and type of a backup job, target repository, number of available and immutable restore points, date and time of the latest and oldest immutable restore points creation.

To get the detailed information on restore points of each workload, click the link in the workload name. The drill-down report page will open.

To get the detailed information on restore points created by a specific backup job, click the link in restore point number. The drill-down report page will open.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

* Business View objects: defines Business View groups to analyze in the report.

* Protected workload types: defines types of protected workloads to analyze in the report (Virtual machine, Computer, Unstructured data, Cloud instance, Enterprise application).
* Job types: defines a job type to analyze in the report (VM backup, Backup copy, Agent backup policy, Agent backup, File backup, Cloud backup policy, Application backup policy, Object Storage backup Cloud Director backup).
* Jobs: defines a list of jobs to analyze in the report.

* Workload exclusion rule: defines a list of workloads that should be excluded from the report scope. You can enter workload names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. Usage example: the following string will exclude workloads with the \_R&D suffix from appearing in the report:\*\_R&D.
* Detailed immutability target: defines whether specific immutability target values must be applied to the analyzed workloads. You can specify target immutability period and number of immutable restore points.

|  |
| --- |
| Note: |
| Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE may show invalid data for Veeam Backup & Replication reports and dashboards. |

[View Report Example](./reports/Immutable%20Workloads.pdf)

Use Case

This report helps to make sure workloads and their backups are safely protected from loss as a result of attacks, malware activity or any other injurious actions.


