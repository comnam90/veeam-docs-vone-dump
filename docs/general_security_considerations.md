---
title: "General Security Considerations"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/general_security_considerations.html"
last_updated: "8/7/2025"
product_version: "13.0.1.6168"
---

# General Security Considerations


General security considerations include best practices which help you to harden Veeam ONE infrastructure, build a more secure environment, and mitigate risks of being compromised. Ensure that your infrastructure meet the common recommendations described in this section. For more information about hardening specific Veeam ONE components, see [Securing Veeam ONE Infrastructure](securing_veeam_one_infrastructure.md).

Network

To secure the communication channel for network traffic, consider the following recommendations:

* Create network segmentation policies to define network boundaries, control traffic between subnets and limit access to security-sensitive Veeam ONE components.
* Make sure that only ports used by Veeam ONE components are opened. For more information, see [Ports](ports.md).
* Use an isolated network to transport data between Veeam ONE components.

* Disable outdated network protocols:

* SSL 2.0 and 3.0 as they have well-known security vulnerabilities and are not NIST-approved. For more information, see [NIST guidelines](https://csrc.nist.gov/publications/detail/sp/800-52/rev-2/final).

* TLS 1.0 and 1.1 if they are not needed. For more information, see [NIST guidelines](https://csrc.nist.gov/publications/detail/sp/800-52/rev-2/final).

* LLMNR and NetBIOS broadcast protocols to prevent spoofing and man-in-the-middle (MITM) attacks.

* SMB 1.0 protocol as it has a number of serious security vulnerabilities including remote code execution. For more information, see [this Microsoft article](https://techcommunity.microsoft.com/t5/storage-at-microsoft/stop-using-smb1/ba-p/425858).

User Permissions

Administrator privileges on the machine where Veeam ONE Server is deployed allow users to access other infrastructure components. If an attacker gains such permissions, they can erase most of the production data as well as compromise other systems in your environment. To mitigate risks, use the principle of least privilege. Provide the minimal required permissions needed for the accounts to operate correctly. For more information, see [Security Groups](security_groups.md) and [Permissions](permissions.md).

File System

Do not add paths writable by untrusted users to the PATH environment variable. A potential attacker may exploit this vulnerability to execute malware or access sensitive data. For more information, see [this CWE article](https://cwe.mitre.org/data/definitions/426.html).

Security Audit

Perform regular security audits to assess your Veeam ONE infrastructure against security criteria and understand if it is compliant with best practices, industry standards, and federal regulations.

To reduce the risk of exploiting vulnerabilities by attackers, follow these recommendations:

* Regularly install the latest security updates and patches on Veeam ONE Server and Veeam ONE components.
* Develop an update management strategy to prevent a negative impact on the production environment.

|  |
| --- |
| Tip: |
| You can subscribe to Veeam security advisories published in the [Veeam Knowledge Base](https://www.veeam.com/knowledge-base.html) to stay up to date with the latest security updates. |

Microsoft Windows Server

To secure Microsoft Windows-based components for Veeam ONE infrastructure, consider the following recommendations:

* Use operating system versions with Long Term Servicing Channel (LTSC). For these versions, Microsoft provides extended support including regular security updates. For more information, see [this Microsoft article](https://docs.microsoft.com/en-us/windows-server/get-started/extended-security-updates-overview).

* Turn on Microsoft Defender Firewall with Advanced Security. Set up rules for inbound and outbound connections according to your infrastructure and Microsoft best practices. For more information, see [this Microsoft article](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-firewall/best-practices-configuring).
* Disable remote services if they are not needed:

* Remote Desktop Service
* Remote Registry service
* Remote PowerShell
* Windows Remote Management service

|  |
| --- |
| Note: |
| Specific Veeam ONE components require additional configuration described in the [Securing Veeam ONE Infrastructure](securing_veeam_one_infrastructure.md) section. |


