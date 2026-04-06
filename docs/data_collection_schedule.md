---
title: "Data Collection Schedule"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/data_collection_schedule.html"
last_updated: "9/22/2025"
product_version: "13.0.1.6168"
---

# Data Collection Schedule


After you connect VMware vSphere, Microsoft Hyper-V, Veeam Backup & Replication and Veeam Backup for Microsoft 365 servers, Veeam ONE will propagate the provided connection settings to all its components and will set up the following default data collection configuration:

* In Veeam ONE Client, the connected servers will be added to the list of monitored objects. Data from the servers will be collected in the real-time mode.

* In Veeam ONE Web Client, the connected servers will be added to the list of objects targeted for data collection. Data collection will be scheduled to run on weekdays, at 3:00 a.m. The first data collection session will start immediately after installation. You can customize the schedule according to which reporting data is collected in the Veeam ONE Web Client console. For details on changing data collection schedule, see [Scheduling Data Collection](schedule_data_collection.md).


