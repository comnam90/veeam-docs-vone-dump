---
title: "Modifying Alarm Assignment Scope"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/modify_alarm_assignment.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Modifying Alarm Assignment Scope


To modify the assignment scope of one or more alarms:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Alarm Management.
2. In the alarm management tree, select the necessary type of infrastructure objects.
3. Select one or more alarms in the list and do either of the following:

* Right-click the alarm and select Edit assignment from the shortcut menu.
* In the Actions pane on the right, click Edit assignment.

1. In the Edit assignment window, select the effective assignment rules and click Remove.
2. Click Add and choose one of the following options:

* Virtual Infrastructure tree — choose this option if you want to assign the alarm to specific levels of the virtual infrastructure.

You can select infrastructure objects that match the alarm type or choose containers from the virtual infrastructure hierarchy. For example, you can assign an alarm of the Virtual Machine type to a specific VM, resource pool, host, cluster, datacenter, or vCenter Server or SCVMM server.

* Business View — choose this option if you want to assign the alarm to custom categorization groups that you have configured in Business View.

For example, if VMs in your environment are divided into SLA groups, you can create a set of alarms that correspond to specific service level requirements and assign these alarms to the necessary SLA group.

* VMware Cloud Director View — choose this option if you want to assign the alarm to a certain level of your VMware Cloud Director infrastructure.

You can select infrastructure objects that match the alarm type or select containers from the VMware Cloud Director hierarchy. For example, you can assign an alarm of the VMware Cloud Director vApp type to a specific vApp, organization VDC, organization or vCloud Director cell.

* Veeam Backup for Microsoft 365 View — choose this option if you want to assign the alarm to a certain level of the Veeam Backup for Microsoft 365 infrastructure.

You can select Veeam Backup for Microsoft 365 infrastructure objects that match the alarm type or select containers from the infrastructure hierarchy. For example, you can assign an alarm of the Repository type to a specific repository or Veeam Backup for Microsoft 365 server.

* Veeam Backup & Replication View — choose this option if you want to assign the alarm to a certain level of the Veeam Backup & Replication infrastructure.

You can select backup infrastructure objects that match the alarm type or select containers from the backup infrastructure hierarchy. For example, you can assign an alarm of the Repository type to a specific repository, Veeam Backup & Replication servers or Veeam Backup Enterprise Manager.

You can combine various types of alarm assignment options for the same alarm. The type of options you can combine depends on the alarm type. For example, if an alarm has the Virtual machine type, you can include in the assignment scope virtual infrastructure, VMware Cloud Director and Business View objects.

1. Repeat steps 3–6 for all virtual and backup infrastructure objects or categorization groups to which the alarms must be assigned.

|  |
| --- |
| ![Modifying Alarm Assignment Scope](images/icon_note.webp) Note: |
| Mind the following restrictions for alarm assignment:   * Alarm can be assigned to infrastructure objects that correspond to the alarm type. For example, alarm of the VM type can be assigned to VMs or to a container that includes VMs. * The same applies to Business View groups: the alarm type must match the Business View category type. You cannot assign an alarm of the Host type to a Business View group that is used to categorize VMs. |


