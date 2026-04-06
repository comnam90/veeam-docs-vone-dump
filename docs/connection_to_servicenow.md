---
title: "Connection to ServiceNow"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/connection_to_servicenow.html"
last_updated: "4/3/2025"
product_version: "13.0.1.6168"
---

# Connection to ServiceNow


The account used to connect to ServiceNow instance must have the following permissions.

* Read permissions on the following tables:

+ /api/now/table/sys\_user

Required to check user availability on the ServiceNow side.

* /api/now/table/sys\_user\_group

Required to check the availability of the assignment group on the ServiceNow side.

* /api/now/table/sys\_choice.\*

Required to check the availability of the close code on the ServiceNow side.

* /api/now/table/incident.\*

* Create permissions on the following tables:

+ /api/now/table/sys\_user.\*
+ /api/now/table/sys\_user

Required to create a Veeam ONE caller in ServiceNow.

* /api/now/table/sys\_user\_group.\*
* /api/now/table/sys\_user\_group

Required to create a Veeam ONE Support group in ServiceNow.

* /api/now/table/incident.\*

* Write permissions on the following tables:

+ /api/now/table/incident.\*
+ /api/now/table/incident.state


