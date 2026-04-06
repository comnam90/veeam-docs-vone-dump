---
title: "Multi-Tenant Monitoring and Reporting"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/multitenant.html"
last_updated: "11/11/2024"
product_version: "13.0.1.6168"
---

# Multi-Tenant Monitoring and Reporting


Veeam ONE supports multi-user access to its monitoring and reporting capabilities. Authorized users can concurrently access the same instance of Veeam ONE to monitor the health state of the virtual infrastructure, view dashboards and run reports.

To restrict access to sensitive infrastructure data, you can limit the scope of virtual infrastructure objects and associated data that must be available to a Veeam ONE user. Thus you can control what subset of the managed virtual infrastructure the user can see and work with.

User permissions can be restricted for two types of inventories only:

* VMware vSphere inventory
* VMware Cloud Director inventory

In a multi-tenant environment, you can configure restricted access to Veeam ONE data for owners of virtualized systems or responsible personnel and delegate monitoring and reporting tasks.

For example, if you manage VMware vSphere systems that belong to different business units, you can restrict permissions so that users can monitor and report on systems owned by their business unit. Or, if you manage resources for multiple organizations in a VMware Cloud Director environment, you can restrict permissions on a per-organization basis, so that users can monitor and report on vApps and VMs that belong to their organization.

This document describes how to configure permissions for multi-tenant monitoring and reporting in Veeam ONE, and provides a basic configuration example.

In This Section

* [How Access to Virtual Infrastructure Objects is Restricted](restricted_access_hiw.md)
* [Permissions and Security Groups](permissions_vs_security_groups.md)
* [Functional Restrictions](functional_restrictions.md)


