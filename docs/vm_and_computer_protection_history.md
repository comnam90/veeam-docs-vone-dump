---
title: "Workload Protection History"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vm_and_computer_protection_history.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Workload Protection History


This report provides historical information on workloads data protection.

* The Summary display includes the following elements:

* The Success and Failure Rates History chart displays the amount of successful and failed resulting job sessions during the reporting period. A resulting job session is the last session started for a job on each day of the reporting period.
* The Success and Failure Rates History table provides information on each day of the reporting period, including number of processed unique workloads, total number of sessions, number of resulting sessions finished successfully, finished with warning and finished with errors, number of running sessions and the percentage of resulting sessions finished successfully and finished with errors.

* The Report Data display provides information on each backup job based on the selected properties.

Veeam Cloud Connect service providers cannot see performance data for proxies used by tenant data protection jobs.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.

* Business View objects: defines a list of Business View objects to include in the report.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Workload types: defines a list of backup infrastructure objects to include in the report (VM, Computer, Unstructured Data, Enterprise Application).
* Job types: defines a list of job types to evaluate in the report (VM backup, Replication, File to tape, Backup to tape, Backup copy, SQL log backup, Oracle log backup, Agent backup policy, Agent backup, File backup, Nutanix AHV backup, Cloud backup policy, Application backup policy, Application backup, PostgreSQL log backup, Cloud Director backup, Cloud Director replication, SOBR sessions: Offload (copy policy), Offload (move policy), Download, Archiving, Retrieval, Object to tape backup, Object storage backup).
* Jobs: defines a list of jobs to include in the report.
* Job statuses: defines a backup job status to analyze in the report (Success, Failed, Warning, Running).
* Job inclusion rule: defines a job to include in the report. You can enter job name explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by comma.
* Period: defines the time period to analyze in the report.

|  |
| --- |
| Note: |
| * Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, you will not be able to generate the report based on Business View objects. * Veeam ONE Web Client displays file backup copy jobs together with other backup copy jobs. |

[View Report Example](./reports/Workload%20Protection%20History.pdf)

Use Case

This report provides historical information on backup sessions for workloads in your backup infrastructure.

Page updated 2026-07-08

