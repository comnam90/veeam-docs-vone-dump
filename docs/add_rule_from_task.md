---
title: "Adding Alarm Rule from Task or Event"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/add_rule_from_task.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Adding Alarm Rule from Task or Event


You can add to an alarm a new rule based on a task or event that occurred in the managed environment. For example, you can create a rule that monitors the Create virtual machine event and notifies you whenever a new VM is created.

To create a new rule from a task or event:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click the necessary view (Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the inventory pane on the left, select the necessary object.
3. In the information pane, open the Tasks & Events tab.
4. Right-click a task or event about which you want to be notified, select Add this event to the existing alarm from the shortcut menu, and click the necessary infrastructure object type.
5. In the Select Alarms window, select an alarm to which the rule must be added and click Add.
6. In the Alarm Settings window, change the rule settings, and click Save.

For details on working with alarm rules, see [Step 3. Specify Alarm Rules and Severity](alarm_rules.md).

1. In the Select Alarms window, click Close.


