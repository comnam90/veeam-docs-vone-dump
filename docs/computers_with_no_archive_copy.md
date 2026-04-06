---
title: "Computers with no Archive Copy"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/computers_with_no_archive_copy.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# Computers with no Archive Copy


The main purpose of backup is to protect your data against disasters and agents failures. Having only one copy of a backup file does not provide the necessary level of safety. To build a successful data protection and disaster recovery plan, you must have at least three copies of your data, for example, production data, backup and its copy, and two different types of media to store copies of your data, for example, disk storage and tape.

To learn more about the 3-2-1 backup strategy, see the Veeam Blog article [How to follow the 3-2-1 backup rule with Veeam Backup & Replication](http://www.veeam.com/blog/how-to-follow-the-3-2-1-backup-rule-with-veeam-backup-replication.html).

This report highlights all agents that do not have backup copies archived to tapes.

|  |
| --- |
| Note: |
| This report does not consider backups stored on cloud backup repositories. |

* The Summary display includes the following elements:

+ The Computers Archive Status chart displays the number of agents with and without archive copy.
+ The Archive Copies by Location Type chart displays the types of backup target locations.
+ The Report Parameters table provides information on the report's configured parameters.

* The Report Data display includes the following elements:

+ Computers with Archive Copy displays data about agent jobs for which a backup copy exists within the specified period.
+ Computers without Archive Copy displays data about agent jobs for which there is no backup copy within the specified period.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Computer type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Backup jobs/policies: defines a list of agent backup jobs to include in the report.

* Agent types: defines types of Veeam backup agents to include in the report.

* Computer inclusion rule: defines names of computers to include in the report.
* Last <N> days/weeks/months: defines the time period to analyze in the report.
* Show computers with no primary backup within the reporting period: defines whether to include in the report agents without primary backup that is valid within the defined time period.

[View Report Example](./reports/Computers%20with%20no%20Archive%20Copy.pdf)

Use Case

This report helps backup administrators check whether agents are protected with backup copies stored on secondary backup repositories and on tape.


