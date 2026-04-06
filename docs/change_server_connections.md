---
title: "Changing Server Connection Settings"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/change_server_connections.html"
last_updated: "9/30/2025"
product_version: "13.0.1.6168"
---

# Changing Server Connection Settings


In some situations, you might need to change connection settings for a monitored server. Consider the following examples:

* If you need to reconnect a server with another user name and/or password, you can change connection settings for this server.
* If the account you provided for a Veeam backup server does not have sufficient permissions to collect data from all backup infrastructure components, you can set custom connection settings for specific servers in your backup infrastructure.

To change connection settings for a server:

1. Open Veeam ONE Web Client.
2. At the top right corner of the Veeam ONE Web Client window, click Configuration.
3. In the Data Collection section of the configuration menu, select your server name.

To narrow down the list, you can either search or apply the following filters:

* In the Status field specify the current operational state of the platform.
* In the Platform type field specify the type of platform in use.
* In the Veeam Analytics service state field specify whether the Veeam Analytics service is running, stopped, or in another state.

1. Click Data source.
2. Click Connection settings.
3. Edit the user name, enter the password and/or change the port number (if applicable).
4. (Optional) If you want to enable Veeam ONE dashboard and report integration in Veeam Backup & Replication, select the Allow Veeam Backup & Replication to display analytics data check box. For details, see [Veeam Backup & Replication Web UI](https://helpcenter.veeam.com/docs/vbr/userguide/vbr_web_console.html?ver=13#analytics).

You can also change connection settings for a server from Veeam ONE Client, to do so:

1. Open Veeam ONE Client.
2. At the bottom of the inventory pane, click Veeam Backup & Replication, Veeam Backup for Microsoft 365, Virtual Infrastructure or VMware Cloud Director.
3. In the inventory pane, right-click the server and choose Connection Settings from the shortcut menu.
4. Edit the user name, enter the password and/or change the port number (if applicable).
5. (Optional) If you want to enable Veeam ONE dashboard and report integration in Veeam Backup & Replication, select the Allow Veeam Backup & Replication to display analytics data check box.

|  |
| --- |
| Note: |
| When changing connection settings, mind the following:   * When you change connection settings for a virtualization server, Veeam ONE disconnects the server and re-connects it with the new settings. When a virtual server is disconnected, previously discovered VMs remain available in the inventory tree. After the server is re-connected, its performance data will be updated. If the connection is not restored, only the history of performance data will be available in Veeam ONE. * When you change connection settings for a backup server in the Veeam Backup Enterprise Manager hierarchy, a new job is automatically configured in Veeam ONE Reporting Sevice to collect data from this backup server. |


