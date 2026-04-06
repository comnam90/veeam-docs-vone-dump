---
title: "Veeam ONE Client"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/silent_install_monitor_ui.html"
last_updated: "9/2/2025"
product_version: "13.0.1.6168"
---

# Veeam ONE Client


To install Veeam ONE Client, use a command with the following syntax:

|  |
| --- |
| msiexec.exe [/L\*v "<path\_to\_log>"] /qn /i "<path\_to\_msi>" [ACCEPT\_THIRDPARTY\_LICENSES="1"][ACCEPT\_EULA="1"][ACCEPT\_REQUIRED\_SOFTWARE="1"][ACCEPT\_LICENSING\_POLICY="1"][INSTALLDIR="<path\_to\_installdir >"][VM\_CLN\_SERVER\_NAME="<one\_server\_address>"] |

The command has the following parameters:

Veeam ONE Client

| Option | Parameter | Required | Description |
| /L | \*v logfile | No | Creates an installation log file with the verbose output.  Specify an existing path to the log file as the parameter value. A setup log file created during the previous installation is cleared.  Example: /L\*v ”C:\ProgramData\Veeam\Setup\Temp\Logs\MonitorClientSetup.txt” |
| /q | n | Yes | Sets the user interface level to “no”, which means no user interaction is needed during installation. |
| /i | setup file | Yes | Installs Veeam ONE Client. Specify a full path to the setup file as the parameter value.  Example: /i “C:\Veeam\Monitor\VeeamONE.Monitor.Client.x64.msi ” |
| ACCEPT\_THIRDPARTY\_LICENSES | 0/1 | Yes | Specifies if you want to accept the terms of the license agreement for the 3rd party components. Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_THIRDPARTY\_LICENSES="1" |
| ACCEPT\_EULA | 0/1 | Yes | Specifies if you want to accept the terms of the Veeam license agreement.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_EULA="1" |
| ACCEPT\_LICENSING\_POLICY | 0/1 | Yes | Specifies if you want to accept the terms of the Veeam licensing policy.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_LICENSING\_POLICY="1" |
| ACCEPT\_REQUIRED\_SOFTWARE | 0/1 | Yes | Specifies if you want to accept the terms of the required software license agreements.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_REQUIRED\_SOFTWARE="1" |
| INSTALLDIR | path | No | Installs the component to the specified location. By default, Veeam ONE uses the Veeam ONE Monitor Client subfolder of the C:\Program Files\Veeam\Veeam ONE folder.  Example: INSTALLDIR="C:\Veeam\"  The component will be installed to the C:\Veeam\Veeam ONE Monitor Client folder. |
| VM\_CLN\_SERVER\_NAME | server name or address | No | Specifies FQDN or IP address of the server where Veeam ONE Client is deployed.  Example: VM\_CLN\_SERVER\_NAME=“oneserver.tech.local" |

Example

Suppose you want to install Veeam ONE Client with the following configuration:

* Installation log location: C:\ProgramData\Veeam\Setup\Temp\Logs\MonitorClientSetup.txt
* No user interaction
* Path to the MSI file: C:\Veeam\Monitor\VeeamONE.Monitor.Client.x64.msi

* Accept 3rd party license agreement
* Accept Veeam license agreement

* Accept required software license agreements
* Accept Veeam licensing policy

* Installation folder: default

* Veeam ONE server: oneserver.tech.local

The command to install Veeam ONE Client with such configuration will have the following parameters:

|  |
| --- |
| msiexec.exe /L\*v "C:\ProgramData\Veeam\Setup\Temp\Logs\MonitorClientSetup.txt" /qn /i "C:\Veeam\Monitor\VeeamONE.Monitor.Client.x64.msi" ACCEPT\_THIRDPARTY\_LICENSES="1" ACCEPT\_EULA="1" ACCEPT\_REQUIRED\_SOFTWARE="1" ACCEPT\_LICENSING\_POLICY="1" VM\_CLN\_SERVER\_NAME="oneserver.tech.local" |


