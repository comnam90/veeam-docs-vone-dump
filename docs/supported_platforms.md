---
title: "Supported Platforms and Applications"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/supported_platforms.html"
last_updated: "2026"
product_version: "13.1.0.7034"
---

# Supported Platforms and Applications


Veeam ONE supports the following virtualization platforms and applications:

VMware vSphere Environment

VMware vSphere Environment

| Specification | Requirement |
| Platforms | * VMware vSphere 9.0 * VMware vSphere 8.0 (up to Update 3) * VMware vSphere 7.0 (up to 7.0 Update 3) * VMware Cloud on AWS |
| Software | * vCenter Server 9.0 * vCenter Server 8.0 (optional\*) (up to 8.0 Update 3) * vCenter Server 7.0 (optional\*) (up to 7.0 Update 3) * Cloud Director 10.4, 10.5, 10.6 |
| Hosts | * ESXi 9.0 * ESXi 8.0 (up to 8.0 Update 3) * ESXi 7.0 (up to 7.0 Update 3)   Note: Free versions of VMware vSphere ESXi are supported. |

|  |
| --- |
| Note: |
| * Only English language versions of VMware infrastructures are supported. * Standalone ESXi hosts are fully supported, so vCenter Server and VMware Cloud Director are optional. However, whenever they are present, we highly recommend that you register both with Veeam ONE. |

\* Adding VMware vSphere infrastructure using vCenter Server is not mandatory.

Microsoft Hyper-V Environment

Microsoft Hyper-V Environment

| Specification | Requirement |
| Platforms | * Windows Server 2025 * Windows Server 2022 * Windows Server 2019 (including 1809) * Windows Server 2016 (including 1709 and 1803) * AzureStack HCI |
| Software | * Microsoft System Center 2025 Virtual Machine Manager (optional\*) * Microsoft System Center 2022 Virtual Machine Manager (optional\*) * Microsoft System Center 2019 Virtual Machine Manager (optional\*) * Microsoft System Center 2016 Virtual Machine Manager (optional\*)   Notes:   * Semi-Annual Channel (SAC) releases are supported. * Adding Microsoft Hyper-V infrastructure using SCVMM is not mandatory. |
| Hosts | * Windows Server Hyper-V 2025 * Windows Server Hyper-V 2022 * Windows Server Hyper-V 2019 * Windows Server Hyper-V 2016   Notes:   * Semi-Annual Channel (SAC) releases are supported. * Free versions of Microsoft Windows Server Hyper-V and Microsoft Hyper-V Server are supported. |

\* Adding Microsoft Hyper-V infrastructure using SCVMM is not mandatory.

Integration with VMware Cloud Director

Veeam ONE offers monitoring and reporting capabilities for VMware Cloud Director version 10.4, 10.5 and 10.6.

Integration with Veeam Backup & Replication

Veeam ONE offers monitoring and reporting capabilities for the following versions of Veeam Backup & Replication and Veeam Backup Enterprise Manager:

* Veeam Backup & Replication 13 (recommended)
* Veeam Backup & Replication 12 or later builds (compatible)

Considerations and Limitations

Consider the following limitations when integrating Veeam Backup & Replication with Veeam ONE:

* Veeam ONE is not compatible with Veeam Backup & Replication versions that are higher than the Veeam ONE version you are using. For example, Veeam Backup & Replication version 13 cannot be added to Veeam ONE version 12.3.
* Monitoring and reporting capabilities depend on licenses installed in Veeam Backup & Replication and Veeam ONE. For details on license compatibility, see [Compatibility with Veeam Backup & Replication Licenses](license_types.md#compatibility).
* Infrastructure topology view in Veeam ONE and Veeam Backup & Replication must match. Otherwise, Veeam ONE Web Client might show invalid data for Veeam Backup & Replication reports and dashboards.
* MFA must be disabled for the account under which Veeam Analytics service connects to Veeam Backup & Replication before installing Veeam Analytics service on the Veeam Backup & Replication server. For details, see section [Disabling MFA for Service Accounts](https://helpcenter.veeam.com/docs/vbr/userguide/mfa.html#disabling-mfa-for-service-accounts) of the Veeam Backup & Replication User Guide.
* It is recommended to install Veeam Analytics service to improve data collection performance in large-scale Veeam Backup & Replication infrastructures. For details on Veeam Analytics service, see [Veeam Intelligent Diagnostics](intelligent_diagnostics.md).
* If you move Veeam Backup & Replication servers to a different Veeam ONE instance and delete from the current instance, the Veeam Backup & Replication servers become unregistered for all integrations. To solve this, clear the Allow Veeam Backup & Replication console to display analytics data check box in Connection Settings and select it in the new Veeam ONE instance. For details, see [Changing Server Connection Settings](change_server_connections.md).

* If you remove Veeam Backup & Replication or Veeam Backup Enterprise Manager servers from Veeam ONE, or remove Veeam Backup & Replication servers from Veeam Backup Enterprise Manager monitored by Veeam ONE, the collected historical data will be lost. This occurs even if the server is added back to Veeam ONE or Veeam Backup Enterprise Manager.

Integration with Veeam Backup for Microsoft 365

Veeam ONE offers monitoring and reporting capabilities for the following versions of Veeam Backup for Microsoft 365:

* Veeam Backup for Microsoft 365 7 or later builds
* Veeam Backup for Microsoft 365 8 or later builds

|  |
| --- |
| Note |
| Before connecting Veeam Backup for Microsoft 365 server to Veeam ONE make sure that:   * License compatibility requirements are met: [Compatibility with Veeam Backup for Microsoft 365 Licenses](license_types.md#vbo). * REST API requirements are met to connect a Veeam Backup for Microsoft 365 server to Veeam ONE: [Configuring REST API and Restore Portal on Separate Machine](https://helpcenter.veeam.com/docs/vbo365/guide/vbo_configuring_rest_separate.html). |

Page updated 2026-07-08

