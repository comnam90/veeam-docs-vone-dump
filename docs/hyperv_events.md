---
title: "Microsoft Hyper-V Tasks & Events"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/hyperv_events.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Microsoft Hyper-V Tasks & Events


You can view information about events that occur in your virtual environment within the selected time interval. Veeam ONE loads information about events through the Event Viewer.

To view the list of events:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Virtual Infrastructure.
2. In the inventory pane, select the necessary infrastructure object.
3. Open the Tasks & Events tab.
4. The Tasks & Events list can display up to 1000 tasks and events at a time. To find the necessary task or event, you can use the following controls:

* To display tasks or events for a specific period, select the necessary time interval from the Events from list.
* To show or hide tasks or events, use filter buttons at the top of the list — Show all events, Show errors, Show warnings, Show info messages, Show user events, Show tasks.
* To find the necessary tasks or events by description, use the Search field at the top of the list.

1. To view the detailed description of an event, click it in the list.

The event description will be shown in the Event Details pane at the bottom.

When you choose a virtual infrastructure container in the inventory pane, you can view events for the selected object and events for its child objects. To hide events related to child objects, clear the Include events from child objects check box at the bottom of the Event Details section.

1. To export displayed events to a CSV file, click the Export to CSV at the top of the list and specify the location where the file will be saved.

[![Hyper-V Tasks & Events](images/hyperv_tasks_and_events.webp)](images/hyperv_tasks_and_events.webp "Hyper-V Tasks & Events")

For every event in the list, the following details are available:

* Event type (User, Info, Warning or Error)
* Short event description
* Time of occurrence
* Event target
* Object that caused or initiated the event


