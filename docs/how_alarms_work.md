---
title: "How Alarms Work"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/how_alarms_work.html"
last_updated: "5/19/2026"
product_version: "13.0.1.6168"
---

# How Alarms Work


After you connect virtual or backup servers, Veeam ONE starts collecting data about objects in your environment and their health state, and checks this data against alarm configuration in real time. If Veeam ONE detects that behavior or state of an infrastructure object meets alarm criteria, or that a specific event occurs, it triggers an alarm with the defined severity level.

After an alarm is triggered, Veeam ONE Client will display alarm details and information about the affected object. You can view, acknowledge or resolve the alarm.

If an alarm is configured to perform an action, Veeam ONE performs a response action after the alarm is triggered — sends an email notification, SNMP trap, or runs a predefined or custom script.

If the event, state or condition that triggered the alarm is resolved, Veeam ONE updates the alarm status in the console.


