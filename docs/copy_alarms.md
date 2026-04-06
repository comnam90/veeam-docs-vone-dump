---
title: "Copying Alarms"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/copy_alarms.html"
last_updated: "3/12/2025"
product_version: "13.0.1.6168"
---

# Copying Alarms


Instead of creating a new alarm from scratch, you can create a copy of an existing alarm and modify its settings.

An alarm copy keeps the same settings as the original alarm, except the alarm assignment. Initially, an alarm copy is not assigned to any virtual infrastructure, VMware Cloud Director objects, Business View groups, or Veeam Backup & Replication and Veeam Backup for Microsoft 365 infrastructure components.

To copy an alarm:

1. Open Veeam ONE Client.

For details, see [Accessing Veeam ONE Components](access.md).

1. At the bottom of the inventory pane, click Alarm Management.
2. Select the necessary alarm in the list.

Press and hold the [CTRL] or [SHIFT] key on the keyboard to select multiple alarms.

1. Do either of the following:

* Right-click the selection and click Copy from the shortcut menu.
* In the Actions pane on the right, click Copy.

What You Can Do Next

After you create an alarm copy, you can change its settings and assignment scope:

1. Select the alarm copy from the list of alarms.

Veeam ONE uses the following pattern for names of alarm copies: Copy of <alarm name>.

1. Change alarm settings and alarm assignment scope.

For details on alarm settings, see [Creating Alarms](create_alarms.md).


