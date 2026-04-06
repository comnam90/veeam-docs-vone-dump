---
title: "Veeam ONE Architecture"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/architecture.html"
last_updated: "10/28/2025"
product_version: "13.0.1.6168"
---

# Veeam ONE Architecture


Veeam ONE relies on client-server architecture to work effectively in environments of any size and complexity. Veeam ONE architecture includes the following structural components:

* Veeam ONE Server

Veeam ONE Server is responsible for collecting data from virtual infrastructure, Veeam Backup & Replication and Veeam Backup for Microsoft 365 servers, and storing this data in the database. As part of Veeam ONE Server, the following components are installed: Veeam ONE Monitoring Service, Veeam ONE Reporting Service, Veeam ONE Error Reporting Service, Veeam ONE Web API and Veeam Analytics service.

* Veeam ONE Web Services

Veeam ONE Web Services enable access to Veeam ONE web server and handle rendering of reports.

* Veeam ONE Client

Veeam ONE Client is a client component of Veeam ONE Server. Veeam ONE Client communicates with the Veeam ONE Server installed locally or remotely.

* Veeam ONE Monitoring Database

Veeam ONE Monitoring database stores data used by product components. The database is hosted on a Microsoft SQL Server that can run remotely, or can be co-installed with other Veeam ONE components.

* Veeam ONE Reporting Database

Veeam ONE Reporting database stores data used by product components. The database is hosted on a PostgreSQL server that can run remotely, or can be co-installed with other Veeam ONE components. Temporary tables are deleted when the Reporter session ends, or after a timeout if the session-based deletion does not occur.

* Veeam Analytics Service

Veeam Analytics service is a component that enables communication with Veeam Backup & Replication servers, collects monitoring and reporting data, and sends remediation commands.

Veeam Analytics service is automatically deployed when you add Veeam Backup & Replication servers to Veeam ONE to improve data collection performance in large-scale Veeam Backup & Replication infrastructures. For details on Veeam Analytics service, see [Veeam Analytics Service](veeam_analytics_service.md) and [Veeam Intelligent Diagnostics](intelligent_diagnostics.md).

Veeam Analytics service can work in the following modes:

* Server

In this mode, Veeam Analytics service is responsible for analyzing logs, data and signature updates.

Veeam Analytics service is included into Veeam ONE installation package and is automatically deployed on the machine running Veeam ONE server during product installation.

* Client

In this mode, Veeam Analytics service is responsible for collecting logs and data and executing remediation actions on Veeam Backup & Replication servers.

By default, Veeam Analytics service client is deployed on Veeam Backup & Replication servers when you connect these servers to Veeam ONE.

Veeam ONE architectural components are installed on a single machine, or run on dedicated machines. For details, see [Deployment Scenarios](deployment_scenarios.md).


