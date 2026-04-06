---
title: "Data Collection"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/one_server_configuration.html"
last_updated: "9/15/2025"
product_version: "13.0.1.6168"
---

# Data Collection


In the Data Collection Overview tab you can configure server connections, Veeam Analytics service settings, Veeam Intelligent Diagnostics settings and perform Advanced actions.

The Overview tab shows overall health status of the connected servers based on collection session and connection status results. In the case of Veeam Backup & Replication servers, it also displays additional information based on the Veeam Analytics service status and state.

If you do not have any connected servers yet, connect them in the Veeam ONE Web Client. For details, see [Add Data Source](connecting_servers.md).

[![Configuration Summary](images/configuration.webp)](images/configuration.webp "Configuration Summary")

For each server in the list, the following details are available:

* Object name
* Platform type
* Status of data source:

* Healthy — no errors detected
* Unhealthy — indicates a problem with data source collection or connection to the server or in the case of Veeam Backup & Replication or Veeam Backup Enterprise Manager, the Veeam Analytics Service is not installed or has connection problems
* Processing — initial data collection is running or status of the data source is synchronizing after services restart

* Veeam Analytics Service state
* Version
* Monitoring Credentials
* Log Analysis Session State
* Log Analysis (enabled or disabled)
* Remediation Actions (enabled or disabled)

Additionally, you can click the Filters button to filter the list by additional details and the Show or hide columns button to broaden or narrow the information displayed. You can also click an individual entry's status to open the Task Details window.

In This Section

* [Adding Data Source](connecting_servers.md)
* [Veeam Analytics Service](veeam_analytics_service.md)
* [Veeam Intelligent Diagnostics](intelligent_diagnostics.md)
* [Advanced Actions](servers.md)
* [Task Sessions](task_sessions.md)


