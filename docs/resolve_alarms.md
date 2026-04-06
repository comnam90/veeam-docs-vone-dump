---
title: "Resolving Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/resolve_alarms.html"
last_updated: "2/3/2025"
product_version: "13.0.1.6168"
---

# Resolving Alarms


Veeam ONE alarms can be resolved automatically or manually.

Alarms are resolved automatically in the following cases:

* When an alarm is disabled or deleted.
* When an object that caused the alarm is deleted or excluded from the alarm assignment scope.
* When conditions that caused the alarm are eliminated, and the alarm is configured to react to this (the alarm resolve action is automatic).

For example, some alarms are configured to change the alarm severity to Resolved in specific cases or during events that occur in the managed infrastructure. Other alarms — such as alarms that are triggered when resource usage is above a certain threshold — are resolved automatically when the resource usage level is back to normal.

You can manually resolve alarms if the state of the monitored object is back to normal, or if the alarm requires no further investigation and no corrective actions should be taken.

In This Section

* [Resolving Individual Alarms](resolve_single_alarms.md)
* [Resolving Multiple Alarms](resolve_multiple_alarms.md)
* [Notifications on Resolved Alarms](resolved_notifications.md)


