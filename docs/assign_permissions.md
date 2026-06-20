---
title: "Step 3. Assign Permissions on Infrastructure Inventory Objects"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/assign_permissions.html"
last_updated: "6/19/2026"
product_version: "13.0.2.6723"
---

# Step 3. Assign Permissions on Infrastructure Inventory Objects


To view and work with virtual infrastructure objects in Veeam ONE, the user must have appropriate permissions on these objects set in the VMware vSphere or VMware Cloud Director inventory.

VMware vSphere Permissions

Connect to vCenter Server or standalone host with vSphere Client and assign permissions on objects to which the user must have access.

The following table shows minimal required privileges on VMware vSphere inventory objects.

VMware vSphere Permissions

| VI Inventory Object | VMware vSphere Privilege |
| vCenter Server (root) Data Center Cluster Host Resource Pool/vApp Datastore Cluster Datastore | Read-only |
| Virtual Machine | * Read-only * Virtual machine.Interaction.Answer question1 * Virtual machine.Interaction.Console interaction1 |

1 Required to access VM console in Veeam ONE Client

|  |
| --- |
| Note: |
| If you assign permissions to container objects (such as hosts, resource pools or vApps), consider enabling propagation. In this case, all new child objects that may be added to the container in future will become available to the user. |

VMware Cloud Director Permissions

Connect to VMware Cloud Director and assign permissions on objects to which the user must have access.

The following table shows minimal required roles for VMware Cloud Director inventory objects.

VMware Cloud Director Permissions

| VI Inventory Object | VMware Cloud Director Role |
| vCloud Director (root) | System Administrator |
| Organization | Console access only |


