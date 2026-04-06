---
title: "Authorizing with Veeam ONE"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/authorization_with_one.html"
last_updated: "1/5/2026"
product_version: "13.0.1.6168"
---

# Authorizing with Veeam ONE


To authorize with Veeam ONE software components (Veeam ONE Client and Veeam ONE Web Client), a user must have the Allow log on locally privilege assigned.

By default, this privilege is assigned to users included in the local Administrators group. For users not included in the local Administrators group, you must assign this privilege manually. For details, see [Microsoft Learn](https://learn.microsoft.com/en-us/windows/security/threat-protection/security-policy-settings/allow-log-on-locally).

|  |
| --- |
| Note: |
| * In the custom deployment scenario, you must assign the Allow log on locally privilege on the machines that host the Veeam ONE Server and Veeam ONE Web Services architectural components. * If the Windows security policy Deny access to this computer from the network is set to deny network logon for local accounts and members of the Administrators group, local administrator accounts may be assigned the Limited Scope user role in Veeam ONE Web Client.   In this situation, Veeam ONE Web Client cannot validate local administrator group membership because it relies on a Windows network logon (Logon Type 3).  To ensure proper validation and access, we recommend using domain accounts or groups for Veeam ONE administration. |


