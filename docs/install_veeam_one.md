---
title: "Installing Veeam ONE"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/install_veeam_one.html"
last_updated: "9/2/2025"
product_version: "13.0.1.6168"
---

# Installing Veeam ONE


This section will guide you through the process of Veeam ONE installation.

Before You Begin

Before you begin installation, check the following prerequisites:

* [Check platform and system requirements](system_requirements.md).

Check that your virtual platform is supported. Make sure the machine where Veeam ONE will be installed meets hardware and software requirements.

* [Check account permissions](permissions.md).

Make sure the user account under which Veeam ONE will be installed has sufficient permissions.

* [Check ports](ports.md).

Make sure all required ports are open for communication between Veeam ONE components, virtualization servers, VMware Cloud Director servers and Veeam Backup & Replication servers.

* Check your Secondary Logon service is enabled

Make sure that your Secondary Logon service is enabled. Disabling a Secondary Logon can affect the installation process if your Veeam ONE service account is different from the account under which the installation wizard is running.

* Download the Veeam ONE installation image file at <https://www.veeam.com/downloads.html>.

Burn the downloaded ISO image file to a CD/DVD or mount the installation image using disk image emulation software. If you install Veeam ONE on a VM, use built-in tools of the virtualization management software to mount the installation image to the VM.

* [Optional] [Creating Veeam ONE Database with SQL Script](create_database_with_sql_script.md).

Normally, the setup automatically creates the Veeam ONE database in the course of installation. However, in some circumstances it might be necessary to create the database with a SQL script instead of using the Veeam ONE Setup wizard. Before installing Veeam ONE, you can create the Veeam ONE database by executing a SQL script that is included with the Veeam ONE installation image.

In This Section

* [All-in-One Installation](typical_installation.md)
* [Custom Installation](advanced_installation.md)
* [Installing Veeam ONE Client](install_monitor_client.md)
* [Installing Veeam ONE in Unattended Mode](silent_mode.md)
* [Upgrading to Veeam ONE 13](upgrade.md)
* [Upgrading Veeam ONE Client](upgrade_monitor_client.md)
* [Uninstalling Veeam ONE](uninstall_veeam_one.md)


