---
title: "Custom Installation"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/advanced_installation.html"
last_updated: "9/29/2025"
product_version: "13.0.1.6168"
---

# Custom Installation


The custom installation scenario implies installing the Veeam ONE Server components (Monitoring service, Reporting service, Veeam ONE Web API) on one machine, and installing the Veeam ONE Web Services component (Veeam ONE Web Client) on another machine. You can also choose to install both components on a single machine in the course of a single installation session. If you choose to install both the Veeam ONE Server and Veeam ONE Web Services components, the custom deployment will mirror the typical, but will not include Veeam ONE Client. You must install Veeam ONE Client separately.

|  |
| --- |
| Important! |
| * If you install the Veeam ONE Server and Veeam ONE Web Services components on separate machines, mind the following limitation: you cannot install the server part on the computer that is already hosting the client part, and conversely.  * If you migrate the Veeam ONE Server components to another machine, you must reinstall Veeam ONE Web Services and specify new connection settings at [Step 11](advanced_connect_server_component.md) of the installation wizard. |

Custom installation is only available if you provide either evaluation or paid license. For Veeam ONE Community Edition, the custom installation option is not available. For details on the custom deployment scenario, see [Custom Deployment](advanced_deployment.md).

The custom installation must proceed in the following order:

1. Install Veeam ONE Server and set up the database.

Run the Veeam ONE Setup wizard on a machine that will host the Veeam ONE Server component. At this step, you must choose existing Microsoft SQL Server and PostgreSQL instances or install new embedded instances and specify the name of the database that will be created by the setup. For details, see [Installing Veeam ONE Server](advanced_server.md).

1. Install the Veeam ONE Web Services.

Run the Veeam ONE Setup wizard on a machine that will host the Veeam ONE Web Services component. For details, see [Installing Veeam ONE Web Services](advanced_web.md).

1. Install and configure Veeam ONE Client.

Run the Veeam ONE Client wizard to enable user access to the Veeam ONE monitoring functionality. If necessary, you can install several instances of Veeam ONE Client on separate machines to provide access to Veeam ONE Client for multiple users. For details, see [Installing Veeam ONE Client](install_monitor_client.md).


