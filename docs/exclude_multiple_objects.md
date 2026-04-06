---
title: "Excluding Multiple Objects from Alarm Assignment Scope"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/exclude_multiple_objects.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Excluding Multiple Objects from Alarm Assignment Scope


You can exclude multiple infrastructure objects from the alarm assignment scope:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Alarm Management.
2. Select the necessary alarm in the list and do either of the following:

* Right-click the alarm and select Edit exclusions from the shortcut menu.
* In the Actions pane on the right, click Edit exclusions.

1. In the Edit exclusions window, click Add and select objects that you want to exclude from the assignment scope:

* Virtual Infrastructure tree — select this option if you want to assign the alarm to specific levels of the virtual infrastructure.

You can select infrastructure objects that match the alarm type or choose containers from the virtual infrastructure hierarchy. For example, you can assign an alarm of the Virtual Machine type to a specific VM, resource pool, host, cluster, datacenter, or vCenter Server or SCVMM server.

* Business View — select this option if you want to assign the alarm to custom categorization groups that you have configured in Business View.

For example, if VMs in your environment are divided into SLA groups, you can create a set of alarms that correspond to specific service level requirements and assign these alarms to the necessary SLA group.

* VMware Cloud Director View — select this option if you want to assign the alarm to a certain level of your vCloud Director infrastructure.

You can select infrastructure objects that match the alarm type or select containers from the vCloud Director hierarchy. For example, you can assign an alarm of the vCloud Director vApp type to a specific vApp, organization VDC, organization or vCloud Director cell.

* Veeam Backup for Microsoft 365 View — select this option if you want to assign the alarm to a certain level of the Veeam Backup for Microsoft 365 infrastructure.

You can select Veeam Backup for Microsoft 365 infrastructure objects that match the alarm type or select containers from the infrastructure hierarchy. For example, you can assign an alarm of the Repository type to a specific repository or Veeam Backup for Microsoft 365 server.

* Veeam Backup & Replication View — select this option if you want to assign the alarm to a certain level of the Veeam Backup & Replication infrastructure.

You can select backup infrastructure objects that match the alarm type or select containers from the backup infrastructure hierarchy. For example, you can assign an alarm of the Repository type to a specific repository, Veeam Backup & Replication servers or Veeam Backup Enterprise Manager.

You can combine various types of alarm assignment options for the same alarm. The type of options you can combine depends on the alarm type. For example, if an alarm has the Virtual machine type, you can include in the assignment scope virtual infrastructure, vCloud Director and Business View objects.

1. Repeat steps 3–4 for all virtual and backup infrastructure objects or categorization groups you want to exclude.
2. In the Edit exclusions window, click OK.

Other Ways to Exclude Multiple Objects from Alarm Assignment

You can also exclude objects from the alarm assignment scope on the Alarms tab of the Virtual Infrastructure view, Business View, VMware Cloud Director view, Veeam Backup for Microsoft 365 view or Veeam Backup & Replication view.

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click the necessary view (Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the inventory pane, select the necessary infrastructure object.
3. In the information pane, open the Alarms tab.
4. Repeat steps 3–5 of the procedure above.


