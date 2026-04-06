---
title: "Connection to Virtualization Servers"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/connection_to_virtual_servers.html"
last_updated: "4/3/2025"
product_version: "13.0.1.6168"
---

# Connection to Virtualization Servers


This section describes permissions to accounts used to connect virtualization servers.

VMware vSphere Servers

The account used to connect vCenter Server and ESXi hosts must have the following privileges:

* Datastore.Browse datastore

Required for collecting datastore details

* Global.Global tag (not required VMware vSphere version 6.5 or later)

Required for running remediation actions

* Global.Licenses

Required for collecting license information

* Host.CIM.CIM Interaction

Required for gathering of ESXi host hardware data

* Host.Configuration.Connection

Required for gathering of ESXi host hardware data

* Host profile.Edit

Required for collecting Host profile properties

* Host profile.View

Required for collecting Host profile properties

* Virtual machine.Interaction.Answer question

Required for using VM Console and viewing snapshot information

* Virtual machine.Interaction.Console interaction

Required for accessing VM console from Veeam ONE Client

* Virtual machine.Snapshot management.Remove Snapshot

Required for running remediation actions

* vSphere Tagging Privileges:

+ vSphere Tagging.Assign or Unassign vSphere Tag
+ vSphere Tagging.Create vSphere Tag
+ vSphere Tagging.Create vSphere Tag Category
+ vSphere Tagging.Delete vSphere Tag
+ vSphere Tagging.Delete vSphere Tag Category
+ vSphere Tagging.Assign or Unassign vSphere Tag on Object

Required for collecting and updating tags on the vCenter Server side. The privileges must be assigned at the vCenter Server level.

|  |
| --- |
| Note: |
| Names of privileges are provided for the latest supported version of VMware vSphere, and may vary for different platform versions. |

Microsoft Hyper-V Hosts and Clusters

The account used to connect standalone Microsoft Hyper-V hosts must:

* Be a member of the Hyper-V Administrators and Performance Monitor Users security groups.
* Have permissions to remotely access WMI on Microsoft Hyper-V hosts.

This includes remote access, activation and launching the DCOM application of WMI, and remote access to the root WMI namespace and sub-namespaces. For details on granting these permissions, see [Configuring Permissions to Remotely Access WMI](access_wmi_remotely.md).

The account used to connect Microsoft Hyper-V clusters must have local Administrator permissions on these clusters.

Microsoft SCVMM

The account used to connect an SCVMM Server must have in SCVMM an assigned user role that is based on the Read-Only Administrator profile.

To monitor clusters and hosts managed by SCVMM, the minimal required permissions for these hosts and clusters must be granted to the same account. For details, see [Microsoft Hyper-V Hosts and Clusters](connection_to_virtual_servers.md#hv).


