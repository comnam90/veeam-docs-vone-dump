---
title: "Permissions and Security Groups"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/permissions_vs_security_groups.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Permissions and Security Groups


Do not mix permissions on virtual infrastructure inventory objects with the Veeam ONE security model that is based on security groups.

Users in Security Groups

Security groups define what actions users can perform in Veeam ONE. That is, what part of Veeam ONE functionality is available to users.

* Veeam ONE Administrators have access to all functions in Veeam ONE. They can perform all types of actions that Veeam ONE supports, including configuration actions.
* Veeam ONE Power Users have read access to monitoring data and can fully manage reports and dashboards but do not have access to Veeam ONE configuration settings.

|  |
| --- |
| Note: |
| Members of the Power Users security group can run report and dashboard scheduling scripts on the machine on which the Veeam ONE Web Services component is installed. Include users into this group with caution. |

* Veeam ONE Read-Only Users have limited access to Veeam ONE functions: they can access data in the read-only mode but cannot perform configuration tasks.

Users included in either Veeam ONE security group (Administrators, Power Users or Read-Only Users) have access to:

* All Veeam ONE consoles (Veeam ONE Client, Veeam ONE Web Client)
* All objects of the infrastructure inventory (including VMware vSphere, VMware Cloud Director, Microsoft Hyper-V, Veeam Backup & Replication and Veeam Backup for Microsoft 365)

Users with Restricted Permissions on Virtual Infrastructure Inventory

Permissions define what part of the virtual infrastructure is visible to a Veeam ONE user. To monitor and report on a restricted subset of the virtual infrastructure in Veeam ONE, a user must have permissions assigned on objects of the VMware vSphere or VMware Cloud Director inventory hierarchy. In this case, the user can utilize Veeam ONE monitoring and reporting capabilities for available objects of the VMware vSphere or VMware Cloud Director infrastructure. Microsoft Hyper-V, Veeam Backup & Replication and Veeam Backup for Microsoft 365 inventory objects are unavailable for the user. For details on limitations of functionality for users with restricted permissions, see [Functional Restrictions](functional_restrictions.md).

|  |
| --- |
| Important! |
| Do not include a user with restricted permissions into Veeam ONE security groups. Members of security groups always have access to the whole infrastructure inventory in Veeam ONE, regardless of their permissions on the VMware vSphere or VMware Cloud Director inventory hierarchy. |

User Permissions

The following table describes what functionality is available to users in accordance with their user role.

Veeam ONE Web Client

Veeam ONE Web Client

| Functionality | Veeam ONE Administrator | Veeam ONE Power User | Veeam ONE Backup Administrator | Veeam ONE Read Only User |
| Threat Center | Full | Full | Read | Read |
| Dashboards | Full | Full | Read | Read |
| Jobs Calendar | Full | Full | N/A | N/A |
| Reports | Full | Full | Read | Read |
| Alarms Overview | Full | Read | Read | Read |
| Scheduling | Full | Limited (Choosing credentials for scheduling is unavailable) | N/A | N/A |
| Deployment Projects | Full | Full | Read | Read |
| Veeam Intelligence | Full | N/A | N/A | N/A |
| Notification Bell | Full | Full | Full | Full |
| Configuration | Full | N/A | N/A | N/A |

Veeam ONE Client

Veeam ONE Client

| Functionality | Veeam ONE Administrator | Veeam ONE Power User | Veeam ONE Read Only User |
| Alarms | Full | Read | Read |
| Infrastructure Changes | Full | N/A | N/A |
| Monitoring | Full | Read | Read |
| Server Settings | Full | N/A | N/A |
| Client Settings | Full | Full | Full |
| Licensing | Full | N/A | N/A |
| Business View | Full | Read | Read |
| Notification Settings | Full | N/A | N/A |
| Credentials Manager | Full | N/A | N/A |

Page updated 2026-07-15

