---
title: "Excluding Single Objects from Alarm Assignment Scope"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/exclude_single_objects.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Excluding Single Objects from Alarm Assignment Scope


You can exclude a single infrastructure object from alarm assignment:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click the necessary view (Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the information pane, open the Alarms tab.
3. Select the necessary alarm in the list and do either of the following:

* Right-click the alarm and select Edit Exclusions from the shortcut menu.
* In the Actions pane on the right, click Edit Exclusions.

If you select a container object and choose an alarm that was triggered for its child object, Veeam ONE will provide two exclusion choices — exclude the child object only or exclude the whole container from the alarm assignment scope.

For example, if in the inventory pane you select a cluster, the list of alarms will contain alarms on the cluster and alarms on the hosts in this cluster. If you select an alarm that was triggered for a host, you can exclude either the host (child object) or the whole cluster (container).

1. Click OK in the dialog box to confirm exclusion.

|  |
| --- |
| ![Excluding Single Objects from Alarm Assignment Scope](images/icon_note.webp) Note: |
| When you exclude an object from an alarm, all unresolved Warning or Error notifications that were triggered by this alarm for the object will change their status to Resolved. |


