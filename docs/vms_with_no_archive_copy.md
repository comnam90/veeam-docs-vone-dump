---
title: "VMs with no Archive Copy"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vms_with_no_archive_copy.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# VMs with no Archive Copy


The main backup purpose is to protect your data against disasters and VM failures. Having only one copy of a backup file does not provide the necessary level of safety. To build a successful data protection and disaster recovery plan, you must have at least three copies of your data, for example, production data, backup and its copy, and two different types of media to store copies of your data, for example, disk storage and tape.

To learn more about the 3-2-1 backup strategy, see the Veeam Blog article [How to follow the 3-2-1 backup rule with Veeam Backup & Replication](http://www.veeam.com/blog/how-to-follow-the-3-2-1-backup-rule-with-veeam-backup-replication.html).

This report analyzes your backup infrastructure to find VMs that do not have backup copies stored on secondary backup repositories or on tapes.

* The Summary section includes the following elements:

+ The VMs by Archive Status chart shows the number of VMs with 1 or 2 archived copies.
+ The VMs per Backup Location chart shows the repositories where backups are stored.

* The Details table shows properties of each protected VMs and provides details on the location of a primary and secondary VM copy, availability of tape backups for the listed VMs and the date of the most recent VM backup.

Report Parameters

You can specify the following report parameters:

* Protected infrastructure: defines the platform to analyze in the report.

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.

* VM folders: defines a list of VMware folders to include in the report (applies to VMware vSphere environments only). VM folders is an alternate way to present the virtual infrastructure. If VMs in your infrastructure are grouped into folders according to their profile, you can limit the report scope by specifying the necessary folders only.

* Business View objects: defines Business View groups to analyze in the report. The parameter options are limited to objects of the Virtual Machine type.

Business View groups from the same category are joined using Boolean OR operator, Business View groups from different categories are joined using Boolean AND operator. That is, if you select groups from the same category, the report will contain all objects that are included in groups. However, if you select groups from different categories, the report will contain only objects that are included in all selected groups.

* VMware Cloud Director objects: defines VMware Cloud Director components to analyze in the report.

* Interval: defines the time period to analyze in the report based on the last backup date of the virtual machine.
* VM exclusion rule: defines a list of VMs that should be excluded from the report scope. You can enter VM names explicitly or create a wildcard mask by using the asterisk (\*) to replace any number of characters. Multiple entries are separated by semicolon. Usage example: the following string will exclude machines with the \_R&D suffix from appearing in the report:\*\_R&D.

[View Report Example](./reports/VMs%20with%20no%20Archive%20Copy.pdf)

Use Case

This report helps backup administrators check whether mission critical VMs are protected with backup copies stored on secondary backup repositories and on tape.


