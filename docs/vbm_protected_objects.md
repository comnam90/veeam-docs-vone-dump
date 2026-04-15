---
title: "Protected Objects (Veeam Backup for Microsoft 365)"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbm_protected_objects.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Protected Objects (Veeam Backup for Microsoft 365)


This report analyzes backup protection of Microsoft 365 objects in your virtual environment.

An object is considered Protected if there is at least one valid backup restore point that meets the designated RPO for it.

The report examines whether objects have valid backup restore points created within the specified time range (RPO period), shows the total number of restore points available for each protected object, and provides information on the completion status of recent backup job sessions.

The report helps you identify which objects in your environment function without proper protection and make sure the existing backups and replicas meet established RPO requirements.

* The Summary display includes the following elements:

+ The Objects by Protection State chart shows the number of protected and unprotected objects.
+ The Objects by Type by Protection State chart shows the number of protected and unprotected objects for each object type.

* The Report Data display provides the User Details, Group Details, Site Details and Teams Details tables that provide information on all protected and unprotected users, groups, sites and teams.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup for Microsoft 365 servers to include in the report.
* Organizations: defines Microsoft organizations to analyze in the report.
* RPO (Recovery Point Objective): defines the maximum amount of data that you may accept to lose, expressed in time. RPO defines the age of the latest backup files required to resume normal operation if system failure occurs. For example, to compile a list of objects protected on a daily basis, you need to set the RPO value to 1 day.
* Object types: defines Microsoft 365 object types to analyze in the report (Users, Groups, Sites, Teams).
* User backup should contain: defines user backup types to analyze in the report (Mailbox, Archive, OneDrive, Site).
* Group backup should contain: defines group backup types to analyze in the report (Group mailbox, Group site).
* Hide objects with no restore point: select the check-box to hide objects with no restore point.

[View Report Example](./reports/Protected%20Objects%20%28Veeam%20Backup%20for%20Microsoft%20365%29.pdf)

Use Case

This report displays a list of Microsoft 365 objects protected by up-to-date backups, as well as a list of unprotected objects which have outdated or missing backups. This information helps you validate the state of backup protection in your organization.


