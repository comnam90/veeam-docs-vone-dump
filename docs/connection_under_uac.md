---
title: "Connection Under UAC"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/connection_under_uac.html"
last_updated: "7/29/2025"
product_version: "13.0.1.6168"
---

# Connection Under UAC


Veeam ONE collects data from Microsoft Windows servers using WMI. For some configurations, UAC access token filtering can prevent running WMI commands on connected machines, which in turn will cause data collection failures. If you are using the default local administrator account, UAC settings do not affect elevation behavior. If you are using a custom local administrator account, you must either configure the LocalAccountTokenFilterPolicy registry key or disable UAC to ensure proper elevation. UAC behavior is affected if a custom user is added to the local Administrators group, regardless of whether Veeam Backup & Replication and Veeam ONE are deployed on the same domain, different domains, or workgroups.

The affected configurations are:

* Non-domain machines (machines in a workgroup)
* Machines with an unelevated local Administrator account (the account that is not Built-in Administrator)

For details on UAC access token filtering, see [Microsoft Learn](https://learn.microsoft.com/en-us/windows/win32/wmisdk/user-account-control-and-wmi).

Machines in a Workgroup

To allow Veeam ONE collect data from machines in a workgroup, perform the following steps:

1. Set the network location to private:

1. Log on to a machine as Administrator.
2. Open the Network & Internet settings.
3. In the list of active networks, click the necessary network and click Properties.
4. Change network profile to Private.

In some Windows OS versions, this location is called Home or Work.

1. To configure Windows Remote Management, in the command prompt, type winrm quickconfig and press [Enter].

Domain Machines

To allow Veeam ONE collect data from domain machines, create the LocalAccountTokenFilterPolicy registry entry on the machine. For details, see this [Microsoft Learn](https://learn.microsoft.com/en-us/troubleshoot/windows-server/windows-security/user-account-control-and-remote-restriction#how-to-disable-uac-remote-restrictions) article.


