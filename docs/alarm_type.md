---
title: "Step 1. Select Alarm Object Type"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/alarm_type.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Step 1. Select Alarm Object Type


All alarms are applied to a certain level of the monitored infrastructure. The Type attribute of an alarm defines to what kind of infrastructure objects this alarm applies. The list of available alarm types is displayed in the inventory pane of the Alarm Management view.

To create a new alarm, select its type first:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Alarm Management.
2. In the alarm management tree, select the necessary object type.
3. In the Actions pane on the right, click the New link.

You can also right-click anywhere in the information pane and choose New from the shortcut menu.

|  |
| --- |
| ![Step 1. Select Alarm Object Type](images/icon_note.webp) Note: |
| Mind that you will not be able to change the alarm type later. |

Creating Alarms from Tasks or Events

You can create an alarm that is based on a task or event that occurred in the monitored infrastructure. Veeam ONE will add the Event-based rule type to the alarm configuration, and will trigger this alarm for all events with the same name. For details on the Event-based rules, see [Adding Event-Based Rules](alarm_rules_events.md).

To create an alarm from a task or event:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. Select the necessary view (Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the information pane, navigate to the Tasks & Events tab.
3. Right-click a task or event for which you want to create an alarm, select Create new alarm from the shortcut menu and then choose an object type.

Creating Alarms from Performance Chart Counters

You can create an alarm from a performance counter. Veeam ONE will add to the alarm configuration a rule based on resource usage counter, and will trigger this alarm every time the counter reaches the specified values. For details on the rules based on resource usage counters, see [Adding Rules Based on Resource Usage Counters](alarm_rules_performance.md).

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. Select the necessary view (Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the object tree, select an object for which you want to create an alarm.
3. Open a tab with performance parameters for which you want to create an alarm (for example, Network, Memory, CPU, and so on).
4. At the bottom of the performance chart, right-click the necessary counter and select Create new alarm from the shortcut menu.

Creating Alarms from In-Guest Processes and Services

You can create an alarm from a process or service. For details on the rules based on specific condition or state, see [Adding State-Based Rules](alarm_rules_state.md).

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. Select the necessary view (Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the object tree, select an object for which you want to create an alarm.
3. Open the Processes or Services tab.
4. Select one or more processes or services in the list.
5. Click the Create Alarm button.

Alternatively, you can right-click the necessary process or service.

1. Select the type of rule on which the alarm must be based.


