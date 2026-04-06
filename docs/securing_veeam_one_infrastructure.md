---
title: "Securing Veeam ONE Infrastructure"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/securing_veeam_one_infrastructure.html"
last_updated: "8/7/2025"
product_version: "13.0.1.6168"
---

# Securing Veeam ONE Infrastructure


This section includes recommendations for hardening specific Veeam ONE components in addition to [general security considerations](general_security_considerations.md).

Infrastructure Planning

For large-scale environments, it is recommended to add Veeam ONE Server and other components to a management domain in a separate Active Directory forest.

For medium-sized and small environments, Veeam ONE components can be placed to a separate workgroup.

In both cases, Veeam ONE components should be placed to a separate network where applicable.

Veeam ONE Server

To secure Veeam ONE Server, consider the following recommendations:

* Restrict outbound connections. To enable product update check, automatic license update, and license usage reporting, Veeam ONE Server must be connected to the internet and be able to send requests to servers on the internet. Allow only HTTPS connections to the Veeam License Update Server (one.butler.veeam.com), Veeam Intelligence endpoints, and Microsoft WSUS servers or Microsoft Update sites.
* Restrict inbound connections. Inbound connectivity to Veeam ONE Server from the internet must not be allowed.

* Restrict collecting data from untrusted Linux VMs. Do not disable SSH fingerprint validation for machines that do not meet specific conditions. For more information, see [Guest OS Credentials](credentials_settings.md).
* Enable automatic update of Veeam Intelligent Diagnostics signatures. To get relevant information about known issues in configuration and performance of backup infrastructure, make sure that Veeam Intelligent Diagnostics signatures are updated regularly. For more information, see [Other Settings](other_settings_server.md).

* Use the recommended Access Control List (ACL) for the custom installation folder. If you specify a custom installation folder for Veeam ONE, use the recommended ACL configuration to prevent privilege escalation and arbitrary code execution (ACE) attacks. Remove all inherited permissions from this folder. Then, add the following permissions:

+ Administrators: Full control, applies to this folder, subfolders and files
+ SYSTEM: Full control, applies to this folder, subfolders and files
+ CREATOR OWNER: Full control, applies to subfolders and files only
+ Users: Read & Execute, applies to this folder, subfolders and files

Veeam ONE Database

The Veeam ONE configuration database stores credentials of user accounts required to connect to virtualization servers and other systems in the backup infrastructure. All passwords stored in the database are encrypted. However, users that have administrator privileges on backup servers can decrypt passwords which is a potential threat.

To secure the Veeam ONE configuration database, consider the following recommendations:

* Check that only authorized users can access Veeam ONE Server and the server that hosts the Veeam ONE configuration database (if the database runs on a dedicated server).
* To protect Veeam ONE data, back up the Veeam ONE database on a regular basis. Also, make sure that the repository for Veeam ONE database backups is not located in the same network with Veeam ONE Server. For more information, see [Database](utility_general.md#db).

Veeam ONE Web Services

The Veeam ONE Web Services component uses Microsoft IIS Web Server. To reduce the attack surface, follow [CIS Benchmark security guidelines](https://www.cisecurity.org/benchmark/microsoft_iis) for your Microsoft IIS version.

Veeam ONE Clients

To secure Veeam ONE clients, consider the following recommendations:

* Use client certificates for user authentication. To protect user accounts with additional user verification, allow users to log in to Veeam ONE Web Client with multi-factor authentication (MFA) through client certificate configuration. For more information, see [Configuring Client Certificate Mapping Authentication](utility_reporter.md#cert).

* Configure user session settings and timeouts. To reduce the number of user sessions opened for a long time in Veeam ONE Client, set the idle timeout to automatically log off users and administrators. Also, limit the number of simultaneous login sessions under the same user credentials to one. For more information, see [Login Sessions](login_session_settings.md).
* Disable multi-tenant access. Restrict access to Veeam ONE Web Client and Veeam ONE Client for users who are not included in Veeam ONE security groups. For more information, see [Other Settings](other_settings_server.md).


