---
title: "Functional Restrictions"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/functional_restrictions.html"
last_updated: "9/30/2025"
product_version: "13.0.1.6168"
---

# Functional Restrictions


Users with restricted permissions on the virtual infrastructure inventory have limited access to Veeam ONE functionality. Functional restrictions prevent these users from changing settings that may affect other users in Veeam ONE.

Veeam ONE Web Client

In Veeam ONE Web Client, users with restricted permissions cannot perform the following tasks:

* Access and modify all configuration settings.
* Modify, delete and schedule predefined and custom dashboards.
* View custom reports that were saved by other users.
* Work with deployment projects.
* Work with specific reports.

For the list of reports available to these users, see [Reports for Users with Restricted Permissions](restricted_access_reports.md).

Users with restricted permissions can access custom dashboards and saved reports that have been shared by Veeam ONE Administrator and Veeam ONE Power User. The virtual infrastructure scope on dashboards and in reports will be restricted in accordance with effective user permissions.

For details on sharing dashboards and reports, see sections [Sharing Dashboards](share_dashboard.md) and [Sharing Reports](publish_reports.md).

Veeam ONE Client

In Veeam ONE Client, users with restricted permissions cannot perform the following tasks:

* Access and modify configuration settings (connections to virtual servers, notification settings, Veeam ONE server settings and license).
* Create, modify, delete, acknowledge or resolve alarms.


