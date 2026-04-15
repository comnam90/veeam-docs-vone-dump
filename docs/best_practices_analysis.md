---
title: "Backup Security and Compliance"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/best_practices_analysis.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Backup Security and Compliance


This report provides information about all backup server configurations to ensure they follow security best practices for the OS and Veeam backup infrastructure components.

* The Summary section includes the following elements:

+ The Backup Server Security & Compliance Status chart shows the status of your total backup servers based on success rate configured in the report's Check result,
+ The Missed Security & Compliance Checks chart shows the volume of missed best practices configured in the report's Check result including whether the security and compliance check missed, is not implemented, is not checked, is suppressed or is unable to detect.
+ The Security & Compliance Last Check chart shows how recently the best practice check was performed on each server.

* The Overview table provides information on security and compliance checks on individual server instances.
* The Details section provides information on best practice types, their status and recommendations on how to resolve best practice failures.

Report Parameters

You can specify the following report parameters to filter your Backup Security & Compliance report:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Best practice types: select the type of the best practice to check for on your servers.
* Check result: filter best practices with the selected states (Passed, Unable to detect, Not implemented, Suppressed, Not checked).

[View Report Example](./reports/Backup%20Security%20and%20Compliance.pdf)

Use Case

This report helps you identify missed security and compliance checks and provides recommendations for rectifying them. Using this report, you can effectively monitor the current status of security and compliance checks within your infrastructure.


