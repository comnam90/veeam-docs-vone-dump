---
title: "Approving Actions for Multiple Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/remediate_multiple_alarms.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Approving Actions for Multiple Alarms


To approve actions for all displayed alarms at once:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click the necessary view (Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the inventory pane, select the necessary object.
3. In the information pane, open the Alarms tab.
4. Use the filters and the search field at the top of the list to display the alarms for which you want to approve actions.

For details on alarm filters, see [Searching for Alarms](view_alarms.md#search).

1. Do either of the following:

* Right-click anywhere in the list of alarms and choose Approve all actions from the shortcut menu.
* In the Actions pane, click Approve All Actions.

1. In the Approve All Actions window, specify a reason or a comment for approving the alarm actions.

The message you specify will appear in the Comment field of the alarm history details, and in the email notification on acknowledged alarms. For details, see [Viewing Alarm History](view_alarm_history.md) and [Notifications on Acknowledged Alarms](acknowledged_notifications.md).

1. Click OK.


