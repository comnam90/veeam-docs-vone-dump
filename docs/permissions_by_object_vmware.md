---
title: "Permissions by Object"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/permissions_by_object_vmware.html"
last_updated: "4/14/2026"
product_version: "13.0.1.6168"
---

# Permissions by Object


This report provides information about permissions assigned in your virtual environment, including individual permissions for every object. The report lists virtual infrastructure objects and shows permissions that each registered user has for these items.

* The Permissions subsections provide information on permissions for each object, including object name, location, user or group, permissions assigned to this user or group and whether permissions can be propagated.

Report Parameters

You can specify the following report parameters:

* Infrastructure objects: defines a virtual infrastructure level and its sub-components to analyze in the report.
* Object name: defines a name of the virtual infrastructure object for which permissions should be shown. You can specify either an exact object name or a part of the name.
* Object type: defines a type of virtual infrastructure objects for which permissions should be shown.
* User/User group: defines a user or a user group for which permissions should be shown.
* User role: defines a user role that should be included in the report.
* Propagated permissions: defines whether permissions that can be propagated to child/dependent objects should be included in the report.

[View Report Example](./reports/Permissions%20by%20Object.pdf)

Use Case

This report helps senior IT administrators review permissions for any given object (vCenter Server, cluster, storage, datacenter, resource pool, vApp, host system or VM).


