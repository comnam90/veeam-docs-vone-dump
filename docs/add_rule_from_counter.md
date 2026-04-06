---
title: "Adding Alarm Rules from Performance Counters"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/add_rule_from_counter.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Adding Alarm Rules from Performance Counters


You can add to an alarm a new rule based on a performance counter.

|  |
| --- |
| ![Adding Alarm Rules from Performance Counters](images/icon_note.webp) Note: |
| You can use this option with objects for which Veeam ONE collects performance data. For objects that do not have any performance data, such as datacenters and clusters, this option is not available. |

To create a new rule from a performance counter:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click the necessary view (Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure, VMware Cloud Director, Business View).
2. In the inventory pane on the left, select the necessary object.
3. Open a tab with performance parameters for which you want to create an alarm (for example, Network, Memory, CPU, and so on).
4. At the bottom of the performance chart, right-click the necessary counter and select Add this counter to the existing alarm from the shortcut menu.
5. In the Select Alarms window, select an alarm to which the rule must be added and click Add.
6. In the Alarm Settings window, change the rule settings, and click Save.

For details on alarm rules, see [Step 3. Specify Alarm Rules and Severity](alarm_rules.md).

1. In the Select Alarms window, click Close.


