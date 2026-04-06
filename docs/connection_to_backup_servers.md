---
title: "Connection to Veeam Backup & Replication Servers"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/connection_to_backup_servers.html"
last_updated: "2/20/2026"
product_version: "13.0.1.6168"
---

# Connection to Veeam Backup & Replication Servers


Veeam Backup server or Enterprise Manager server on Microsoft Windows

To connect Veeam Backup & Replication servers you must specify:

1. Veeam Analytics service deployment credentials:

* This account must have an access to the administrative share on the machine where Veeam Analytics service is deployed.

1. Backup Monitoring credentials:

* This account must have the Veeam Backup Administrator role assigned.

This role must be assigned to the account on the machine that runs Veeam Backup & Replication.

* Must be a member of the Performance Monitor Users and Event Log Readers security groups.

These permissions must be granted to the account on machines that run:

* Veeam Backup & Replication on Microsoft Windows.
* Backup proxy, backup repository, WAN Accelerator, tape server and cloud gateway components (Windows-based) (required to collect performance data from these servers).

* Must have permissions to remotely access WMI.

This includes remote access, activation and launching the DCOM application of WMI, and remote access to the root WMI namespace and sub-namespaces. For details on granting these permissions, see [Configuring Permissions to Remotely Access WMI](access_wmi_remotely.md).

This permission must be granted to the account on machines that run:

* Veeam Backup & Replication on Microsoft Windows.
* Backup proxy, backup repository (Windows-based), WAN Accelerator, tape server and cloud gateway components (required to collect performance data from these servers).

|  |
| --- |
| Note: |
| You must use the account with local Administrator permissions in the following cases:   * When you install Veeam Analytics service on a Veeam Backup & Replication server you must disable MFA for the account under which Veeam Analytics service connects to Veeam Backup & Replication. For details, see section [Disabling MFA for Service Accounts](https://helpcenter.veeam.com/docs/vbr/userguide/mfa.html#disabling-mfa-for-service-accounts) of the Veeam Backup & Replication User Guide. * If machines that run Veeam ONE server and Veeam Backup & Replication server belong to different domains or workgroups. * If you are using the default local administrator account, UAC settings do not affect elevation behavior. If you are using a custom local administrator account, you must either configure the LocalAccountTokenFilterPolicy registry key or disable UAC to ensure proper elevation. UAC behavior is affected if a custom user is added to the local Administrators group, regardless of whether Veeam Backup & Replication and Veeam ONE are deployed on the same domain, different domains, or workgroups. |

Veeam Backup server or Enterprise Manager server on Linux

To connect Veeam Backup & Replication servers you must specify:

* Veeam Analytics service deployment credentials.

This account must have the Veeam Backup Administrator role assigned.

This role must be assigned to the account on the machine that runs Veeam Backup & Replication.

|  |
| --- |
| Note: |
| You must use the account with local Administrator permissions in the following cases:   * When using a user account other than the default veeamadmin, it is recommended to assign the Service Account role in Veeam Host Management and also Veeam Backup Administrator permissions in Veeam Backup & Replication. For details on roles and permissions, see [Configuring Users](https://helpcenter.veeam.com/docs/vbr/userguide/hmc_configure_users.html) and [Configuring Roles](https://helpcenter.veeam.com/docs/vbr/userguide/configure_roles.html) in the Veeam Backup & Replication User Guide.   For newly created local users in Veeam Host Management with a role other than Service Account, the user must first log in to the Veeam Software Appliance Web Client to change the password. Otherwise, an error occurs when connecting to the backup server to deploy Veeam Analytics service. |


