---
title: "Adding Rules Based on Resource Usage Counters"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/alarm_rules_performance.html"
last_updated: "5/12/2025"
product_version: "13.0.1.6168"
---

# Adding Rules Based on Resource Usage Counters


Alarms with rules resource usage counters alert about the important changes in the performance of objects from the monitored infrastructure.

To add a rule based on resource usage counters:

1. On the Rules tab, click Add.
2. At the Choose Rule Type step of the wizard, select Resource usage.
3. At the Define Rule step of the wizard, specify conditions (or other settings, as applicable) for the alarm rule.

If you want to put the rule in action for the alarm, make sure that the Enable this rule check box is selected. If you unselect this check box, the rule settings will be saved, but the rule will be disregarded.

1. [Optional] Exclude specific objects from the alarm scope.

By default, counter-based rules apply to all storage objects in the alarm scope. For example, if you create an alarm rule for a host and select a datastore usage counter, this rule will apply to all datastores connected to the host.

For some counter-based rules, you can exclude specific storage objects from the alarm scope. Excluded objects will not be monitored by the alarm. To exclude one or more storage objects, specify their names in the Exclude instances field. Separate object names with a semicolon (;).

|  |
| --- |
| ![Adding Rules Based on Resource Usage Counters](images/icon_note.webp) Note: |
| * When you specify objects to exclude, use object display names. To learn the exact display name of an object, navigate to a performance chart for the necessary object in Veeam ONE Client, and choose a chart view with the necessary counter. You can check the object display name either in the chart legend or in the Select Devices and Counters window > Devices list. For details, see [Selecting Chart Views and Performance Counters](select_vsphere_counters.md).  * Names of drives must be specified with the backward slash, for example, C:\; Z:\. |

1. Click Finish.
2. Repeat steps 1–5 for every alarm-based rule you want to add.


