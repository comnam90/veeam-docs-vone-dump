---
title: "Step 2. Check Requirements to User Account"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/check_account_requirements.html"
last_updated: "5/5/2026"
product_version: "13.0.1.6168"
---

# Step 2. Check Requirements to User Account


You can provide access to Veeam ONE for single users and user groups.

The following table describes types of accounts for which you can configure restricted permissions.

Step 2. Check Requirements to User Account

| Platform | Account Type | Description and Notes |
| vCenter Server | Domain users and groups | Members of the Active Directory domain.  vCenter Server must be configured to use Active Directory for authentication. For details on user authentication in VMware vSphere, see [Active Directory Identity Source Settings](https://docs.vmware.com/en/VMware-vSphere/6.7/com.vmware.psc.doc/GUID-4D24C6E8-63F5-4E35-862E-B59A03703254.html).  To log in to Veeam ONE, you must provide user name in the following format: domain\username. |
| Local users and groups | Local users and groups on the machine where vCenter Server is installed.  To log in to Veeam ONE, you must provide user name in the following format: hostname\username. |
| Single Sign-On users and groups | Single Sign-On users and groups on vCenter Server. For details, see [vSphere Authentication with vCenter Single Sign-On](https://docs.vmware.com/en/VMware-vSphere/6.7/com.vmware.psc.doc/GUID-B98DF9C2-FE7D-483F-9521-C17C138B59D8.html).  Note: Single Sign-On must be installed on the machine where vCenter Server runs, with the default installation path and port settings. Otherwise, Veeam ONE will not be able to detect its database with user groups and users.  To log in to Veeam ONE, you must provide user name in the following format: ssodomain\username. |
| ESXi host | Domain users and groups | Members of the Active Directory domain.  Standalone hosts must be configured to use Active Directory for authentication. For details, see [Using Active Directory to Manage ESXi Users](https://docs.vmware.com/en/VMware-vSphere/6.7/com.vmware.vsphere.security.doc/GUID-4FD32125-4955-439D-B39F-C654CCB207DC.html?hWord=N4IghgNiBcIKoGcCWA7A5gAgIIGMAuSAbgKYYAiSATsfgPaUCeGetGAsmCmGqQKIDKADSQZExSghABfIA).  To log in to Veeam ONE, you must provide user name in the following format: domain\username. |
| VMware Cloud Director | Domain users and groups | Members of the Active Directory domain.  Users must be able to authenticate to an LDAP server. For details, see [VMware Cloud Director documentation](https://docs.vmware.com/en/VMware-Cloud-Director/10.3/VMware-Cloud-Director-Service-Provider-Admin-Portal-Guide/GUID-4ECA36E9-E051-489C-A039-67621DE2C688.html#GUID-4ECA36E9-E051-489C-A039-67621DE2C688).  To log in to Veeam ONE, you must provide user name in the following format: domain\username. |
| Local users and groups | Local users and groups in VMware Cloud Director.  To log in to Veeam ONE, you must provide user name in the following format:   * For organization user: organization\username * For VMware Cloud Director administrator: system\username |

|  |
| --- |
| Note: |
| For each local or Single Sign-On user that authenticates to Veeam ONE, Veeam ONE creates a temporary Windows account on the machine that runs the Veeam ONE Server component. This temporary account is deleted after 30 days of inactivity. |

Authorizing with Veeam ONE

To authorize with Veeam ONE components (Veeam ONE Client and Veeam ONE Web Client), a user must have the Allow log on locally privilege assigned.

By default, this privilege is assigned to users included in the local Administrators group. For users not included in the local Administrators group, you must assign this privilege manually.

|  |
| --- |
| Note: |
| If you use the advanced deployment scenario, you must assign the Allow log on locally privilege on the machines that host the Veeam ONE Server and Veeam ONE Web UI components. |


