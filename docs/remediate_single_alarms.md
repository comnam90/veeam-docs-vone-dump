---
title: "Approving Actions for Individual Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/remediate_single_alarms.html"
last_updated: "10/1/2025"
product_version: "13.0.1.6168"
---

# Approving Actions for Individual Alarms


You can approve individual alarms in both Veeam ONE Client and the Veeam ONE Web Client Alarms Overview screen.

Approving actions for alarms in Veeam ONE Web Client

To approve individual alarms in the Veeam ONE Web Client Alarms Overview:

1. Open Veeam ONE Web Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. Open the Alarms Overview section.
2. Click the Filters button at the top of the screen and click the Only alarms with remediation check box.
3. Click Apply.
4. In the filtered alarm list at the bottom of the screen, click on your desired alarm.
5. On the alarm details window, click Approve Action.
6. In the Approve Action window, specify a comment or a reason for approving the alarm.
7. Click OK.

Approving actions for alarms in Veeam ONE Client

To approve actions for individual alarms:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click the necessary view (Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the inventory pane, select the necessary object.
3. In the information pane, open the Alarms tab.
4. At the top of the alarms list, click the Show alarms with available Remediation Actions icon.
5. In the list of alarms, select one or more alarms and do either of the following:

* Right-click the selection and choose Approve action from the shortcut menu.
* In the Actions pane, click Approve Action.

Press and hold the [CRTL] or [SHIFT] key to select multiple alarms.

1. In the Approve Action window, specify a reason or a comment for approving the alarm actions.

The message you specify will appear in the Comment field of the alarm history details, and in the email notification on acknowledged alarms. For details, see [Viewing Alarm History](view_alarm_history.md) and [Notifications on Acknowledged Alarms](acknowledged_notifications.md).

1. Click OK.


