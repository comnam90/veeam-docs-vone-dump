---
title: "Tenants Backup Compatibility"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/tenants_backup_compatibility.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Tenants Backup Compatibility


This report shows what versions of Veeam Backup & Replication run on backup servers of Veeam Cloud Connect tenants.

* The Details section shows a list of tenants and version and build number of Veeam Backup & Replication running on tenants backup servers.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a list of Veeam Backup & Replication servers to include in the report.
* Tenants: defines a list of Veeam Cloud Connect tenants to include in the report.

[View Report Example](./reports/Tenants%20Backup%20Compatibility.pdf)

Use Case

If the service provider runs the latest version of Veeam Backup & Replication, it is recommended that tenants connected to this service provider also upgrade to the latest version of Veeam Backup & Replication. Tenants who run an earlier version of Veeam Backup & Replication cannot leverage the full cloud connect functionality, as features introduced in the latest version will not work for them and may result in failed jobs.

For details, see section [Console Versions in Veeam Cloud Connect Infrastructure](https://helpcenter.veeam.com/docs/backup/cloud/cloud_connect_versions.html) of the Veeam Cloud Connect Guide.


