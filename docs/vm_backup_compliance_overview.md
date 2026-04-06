---
title: "VM Backup Compliance Overview"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vm_backup_compliance_overview.html"
last_updated: "3/30/2026"
product_version: "13.0.1.6168"
---

# VM Backup Compliance Overview


This report returns a list of VMs that do not meet the requirement to have a minimal number of available backup copies.

To learn more about the 3-2-1 backup strategy, see the Veeam Blog article [How to follow the 3-2-1 backup rule with Veeam Backup & Replication](http://www.veeam.com/blog/how-to-follow-the-3-2-1-backup-rule-with-veeam-backup-replication.html).

* The Summary section includes the VM Compliance Status chart that shows the proportion of backup-compliant VMs to the rest of VMs across the selected virtual infrastructure scope.
* The Details table provides information on non-compliant VMs properties, including VM location, number of backup copies/replicas, backup type and the date of the latest backup.

Report Parameters

You can specify the following report parameters:

* Protected infrastructure: defines the platform to analyze in the report.
* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* VM folders: defines a list of VMware folders to include in the report (applies to VMware vSphere environments only). VM folders is an alternate way to present the virtual infrastructure. If VMs in your infrastructure are grouped into folders according to their profile, you can limit the report scope by specifying the necessary folders only.
* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.
* Required number of VM copies: defines the minimum number of backup copies/replicas a virtual machine must have to meet the compliance requirements.
* VM exclusion rule: defines a list of VMs that should be excluded from the report scope. You can enter VM names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. Usage example: the following string will exclude machines with the \_R&D suffix from appearing in the report:\*\_R&D.

[View Report Example](./reports/VM%20Backup%20Compliance%20Overview.pdf)

Use Case

This report allows you to make sure that all mission critical VMs have sufficient amount of backup copies in distinct locations within the organization, as requested by the 3-2-1 backup strategy. This information may help you modify job settings or dynamically adjust your backup file retention policies.


