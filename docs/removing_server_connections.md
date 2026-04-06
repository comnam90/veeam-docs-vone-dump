---
title: "Removing Server Connections"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/removing_server_connections.html"
last_updated: "10/1/2025"
product_version: "13.0.1.6168"
---

# Removing Server Connections


If you no longer want to monitor a virtualization or a backup server, you can remove a connection to it in Veeam ONE Client.

To change connection settings for a server:

1. Open Veeam ONE Web Client.
2. At the top right corner of the Veeam ONE Web Client window, click Configuration.
3. In the Data Collection section of the configuration menu, select your server name.

To narrow down the list of servers, you can either search or apply the following filters:

* In the Status field specify the current operational state of the platform.
* In the Platform type field specify the type of platform in use.
* In the Veeam Analytics service state field specify whether the Veeam Analytics service is running, stopped, or in another state.

1. Click Data source.
2. Click Remove server.

You can also remove data sources from Veeam ONE Client, to do so:

1. Open Veeam ONE Client.
2. At the bottom of the inventory pane, click Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure or VMware Cloud Director.
3. In the inventory pane, right-click the server you want to remove and choose Remove Server from the shortcut menu.

After you remove a server connection in Veeam ONE Client, connection to this server will be automatically removed in Veeam ONE Reporting Service.

|  |
| --- |
| Note: |
| When removing server connection, mind the following:   * When you remove a server, historical performance and configuration data for the server and its child objects is deleted from the Veeam ONE database. * When you remove VMware Cloud Director, Veeam ONE withdraws connection to VMware Cloud Director server only. Connections to underlying vCenter Servers are not removed automatically — you must remove these connections manually. * When you delete Veeam Backup & Replication, Veeam ONE becomes unregistered on Veeam Backup & Replication for dashboards and reports integrations and additionally reports saved from Veeam Backup & Replication Analytics nodes are also removed. For details on Veeam Backup & Replication Analytics, see [Veeam Backup & Replication Web UI](https://helpcenter.veeam.com/docs/vbr/userguide/vbr_web_console.html?ver=13#analytics). |


