---
title: "Connection to Microsoft SQL Server"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/connection_to_sql.html"
last_updated: "2/5/2026"
product_version: "13.0.1.6168"
---

# Connection to Microsoft SQL Server


The account used to connect to the Microsoft SQL Server hosting the Veeam ONE database during installation must have the following permissions:

* Public role — default permissions for SQL users
* CREATE ANY DATABASE permissions — required for database creation during setup
* db\_owner role on the Veeam ONE database — required for communication of Veeam ONE services with the database
* db\_datareader permissions on the master database — required to verify that only one product installation writes data to the database
* public, db\_datareader, SQLAgentUserRole permissions on the msdb database — required for setup and database index optimization
* [For Always-On Availability Groups] VIEW SERVER STATE, VIEW ANY DEFINITION permissions — required to check database existence and to verify that Veeam ONE will write data to the primary replica of the database

After installation, the account used for upgrades and communication of Veeam ONE services with Veeam ONE database must have the following permissions:

* Public role (default permissions)
* db\_owner role on the Veeam ONE database
* db\_datareader permissions on the master database
* [For Always-On Availability Groups] VIEW SERVER STATE, VIEW ANY DEFINITION permissions

For details on permission requirements for SQL Server Reporting Services connection, see [Configuring SSRS Server Settings](configure_ssrs_server_settings.md).


