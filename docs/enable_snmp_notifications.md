---
title: "Step 3. Enable SNMP Notification for Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/enable_snmp_notifications.html"
last_updated: "10/3/2025"
product_version: "13.0.1.6168"
---

# Step 3. Enable SNMP Notification for Alarms


To receive SNMP traps when an alarm is triggered, you must set SNMP notification as a response action for every alarm manually.

To configure SNMP traps for an alarm:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Alarm Management.
2. To open the Alarm Settings window for the necessary alarm, do either of the following:

* Double click the necessary alarm in the list.
* Right-click the alarm and choose Edit from the shortcut menu.
* Select the alarm in the list and click Edit in the Actions pane on the right.

1. In the Alarm Settings window, open the Notifications tab.
2. On the Notifications tab, click Add.
3. From the Action list, select Send SNMP trap.
4. From the Condition list, choose the severity of alarms about which recipients must be notified:

+ Any state — an SNMP trap will be sent every time when an alarm status changes to Error, Warning, Info or Resolved.
+ Errors and warnings — an SNMP trap will be sent every time when an alarm status changes to Error or Warning.
+ Resolved — an SNMP trap will be sent every time when an alarm status changes to Resolved.
+ Errors only — an SNMP trap will be sent every time when an alarm status changes to Error.

1. Click Save.

[![Click the image to zoom in](images/set_trap_action.webp)](images/set_trap_action.webp "Click the image to zoom in")


