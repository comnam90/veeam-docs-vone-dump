---
title: "Alarm Notification Options"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/notification.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Alarm Notification Options


You can configure Veeam ONE to send notifications when alarms are triggered or change their status. Depending on alarm configuration, Veeam ONE can:

* Send email notifications to the default notification group or to specific recipients
* Send SNMP traps to third-party consoles

Alarm notification options are defined in alarm settings. You can specify when Veeam ONE must notify you about alarm status change:

* Alarm severity changes to Error
* Alarm severity changes to Error or Warning
* Alarm is resolved
* Alarm severity changes to any level (Error, Warning or Resolved)

By default, all predefined alarms are configured to send email notifications to the default notification group when the alarm severity changes to any level. You can change alarm notification settings and define conditions when notifications must be sent.

Related Topics

[Configuring Alarm Notifications](configure_alarm_notification.md)

Page updated 2026-08-05

