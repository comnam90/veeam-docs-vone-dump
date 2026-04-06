---
title: "Veeam Backup for Microsoft 365 Events"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/vbo_events.html"
last_updated: "8/7/2025"
product_version: "13.0.1.6168"
---

# Veeam Backup for Microsoft 365 Events


The Tasks & Events dashboard shows the history of events that triggered Veeam Backup for Microsoft 365 alarms. For the list and detailed description of data protection alarms, see [Veeam Backup for Microsoft 365 Alarms](vbm_alarms_events.md).

To view the list of events for a specific level:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Veeam Backup for Microsoft 365.
2. In the inventory pane, select the necessary backup infrastructure node.
3. Open the Tasks & Events tab.
4. The Tasks & Events list can display up to 1000 tasks and events at a time. To find the necessary task or event, you can use the following controls:

* To display tasks or events for a specific period, select the necessary time interval from the Events from list.
* To show or hide tasks or events, use filter buttons at the top of the list — Show all events, Show errors, Show warnings, Show info messages, Show user events, Show tasks.
* To find the necessary tasks or events by description, use the Search field at the top of the list.

1. To view the detailed description of an event, click it in the list.

The event description will be shown in the Event Details pane at the bottom.

When you choose a virtual infrastructure container in the inventory pane, you can view events for the selected object and events for its child objects. To hide events related to child objects, clear the Include events from child objects check box at the bottom of the Event Details section.

1. To export displayed events to a CSV file, click Export to CSV at the top of the list and specify the location where the file will be saved.


