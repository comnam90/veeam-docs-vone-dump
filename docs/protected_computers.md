---
title: "Protected Computers"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/protected_computers.html"
last_updated: "4/20/2026"
product_version: "13.0.1.6168"
---

# Protected Computers


This report provides information on all protected and unprotected computers including their last backup state.

A computer is considered to be Protected if there is at least one valid backup restore point that meets the designated RPO for it. A computer is considered to be Unprotected if it has an outdated or missing backup restore point.

The report examines whether computers have valid backup restore points created within the specified time range (RPO period), shows the total number of restore points available for each protected computer, and provides information on the completion status of recent backup job sessions.

* The Summary display contains the following charts:

+ The Protected Computers chart shows the number of protected and unprotected computers.
+ The Computer Type chart shows types of protected computers.
+ The Computer Last Backup State chart shows status of the latest job session for a discovered/protected computer.
+ The Unprotection Reason chart shows reasons for non-compliance with the specified RPO requirements.
+ The Report Parameters and Summary panels show the specific configured parameters for the report and provide information on the number of discovered, backed up and protected computers.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers and protection groups to include in the report.
* Business View objects: defines a list of business groups to include in the report. The parameter options are limited to objects of the Computer type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* Backup jobs/policies: defines a list of backup jobs and policies to include in the report.
* Agent types: defines types of Veeam backup agents to include in the report.
* Computer inclusion rule: defines names of computers that must be included in the report.

In the Computer inclusion rule field, you can specify a mask for names of computers that must be included in the report scope. The mask can contain the asterisk (\*) that stands for zero or more characters. You can specify multiple masks or computer names separated with commas.

* RPO (Recovery Point Objective): defines the maximum amount of data that you may accept to lose, expressed in time. RPO defines the age of the latest backup files required to resume normal operation if system failure occurs. For example, to compile a list of computers protected on a daily basis, you need to set the RPO value to 1 day.

[View Report Example](./reports/Protected%20Computers.pdf)

Use Case

When you set up your agent backup jobs based on protection groups or employ complex exclusion parameters in job properties, some computers may turn out to be excluded from protection groups and therefore will lack proper protection.

This report displays a list of computers protected by up-to-date backups as well as a list of unprotected computers which have outdated or missing backups. This information helps you identify which computers in your environment function without proper protection and make sure the existing backups meet established RPO requirements.


