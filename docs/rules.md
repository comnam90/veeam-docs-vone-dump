---
title: "Alarm Rules"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/rules.html"
last_updated: "9/14/2023"
product_version: "13.0.1.6168"
---

# Alarm Rules


Every alarm has one or more associated rules that define conditions to trigger the alarm, severity of the alarm and rule suppression settings.

There are the following types of alarm rules:

* Event-based rules are rules for alerting about specific events that occur in the backup or virtual infrastructure. These can be events issued by the hypervisor or Veeam Backup & Replication events.
* Rules for a specific condition or state are rules for alerting about important conditions or changed state of infrastructure objects.
* Rules based on existing alarms are rules for alerting about other alarms triggered in Veeam ONE.
* Rules based on resource usage counters are rules for alerting about abnormal resource usage of infrastructure objects.

For the full list of available rule types, see [Alarm Rules Reference](appendix_rules_alarms.md).

Aggregation Type

An aggregation type defines how Veeam ONE analyzes performance data collected for a specified period of time, and compares it to the threshold.

The following table explains how Veeam ONE alarms trigger depending on the aggregation type and rule condition:

Aggregation Type

| Aggregation Type | Condition | |
| Above | Below |
| Min | Veeam ONE takes the minimum value across the collected performance parameters and compares it to the specified threshold. If the value is above the threshold, Veeam ONE triggers an alarm. That means that the alarm triggers only if all the values are above the threshold. | Veeam ONE takes the minimum value across the collected performance parameters and compares it to the specified threshold. If the value is below the threshold, Veeam ONE triggers an alarm. That means that the alarm triggers if at least one of the collected values is below the threshold. |
| Avg | Veeam ONE takes the average value across the collected performance parameters. The alarm triggers if this value is above the threshold. | Veeam ONE takes the average value across the collected performance parameters. The alarm triggers if this value is below the threshold. |
| Max | Veeam ONE takes the maximum value across the collected performance parameters and compares it to the specified threshold. If the value is above the threshold, Veeam ONE triggers an alarm. That means that the alarm triggers if at least one of the collected values is above the threshold. | Veeam ONE takes the maximum value across the collected performance parameters and compares it to the specified threshold. If the value is below the threshold, Veeam ONE triggers an alarm. That means that the alarm triggers only if all the values are below the threshold. |

To learn how to configure rules based on performance counters, see [Adding Rules Based on Resource Usage Counters](alarm_rules_performance.md).

Analysis Depth

Alarm rules may include the Analysis depth parameter. This parameter defines the number of latest performance data values among which an average value is calculated. Each newly collected value is compared to the average value. If the new value is above or below the average value according to severity levels, Veeam ONE triggers the alarm.

Linking Rules

You can link two or more rules using Boolean operators:

* AND — if rules are joined with this operator, an alarm is triggered when conditions for all linked rules are met.
* OR — if rules are joined with this operator, an alarm is triggered when a condition for any of the linked rules is met.

You can form several groups of linked rules and join them with different operators. To learn how to link rules, see [Linking Rules](alarm_rules_link.md).


