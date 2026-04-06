---
title: "Veeam Analytics Service"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/silent_install_agent.html"
last_updated: "9/2/2025"
product_version: "13.0.1.6168"
---

# Veeam Analytics Service


To install Veeam Analytics service, use a command with the following syntax:

|  |
| --- |
| msiexec.exe [/L\*v "<path\_to\_log>"] /qn /i "<path\_to\_msi>" [ACCEPT\_THIRDPARTY\_LICENSES="1"][ACCEPT\_EULA="1"][ACCEPT\_REQUIRED\_SOFTWARE="1"][ACCEPT\_LICENSING\_POLICY="1"][INSTALLDIR="<path\_to\_installdir >"][VO\_AGENT\_TYPE="1"][VO\_AGENT\_SERVICE\_ACCOUNT\_NAME="<Veeam\_One\_Service\_Account>"][VO\_AGENT\_SERVICE\_ACCOUNT\_PASSWORD="<Veeam\_One\_Service\_Account\_Password>"][VO\_BUNDLE\_INSTALLATION="1"] [VO\_AGENT\_SERVICE\_PORT="<agent\_port>"] |

|  |
| --- |
| Important! |
| Veeam Analytics service server component must be installed on the machine that runs Veeam ONE server components. |

The command has the following parameters:

Veeam Analytics Service

| Option | Parameter | Required | Description |
| /L | \*v logfile | No | Creates an installation log file with the verbose output.  Specify an existing path to the log file as the parameter value. A setup log file created during the previous installation is cleared.  Example: /L\*v ”C:\ProgramData\Veeam\Setup\Temp\Logs\AgentSetup.txt” |
| /q | n | Yes | Sets the user interface level to “no”, which means no user interaction is needed during installation. |
| /i | setup file | Yes | Installs Veeam ONE Client Client. Specify a full path to the setup file as the parameter value.  Example: /i “C:\Veeam\Monitor\VeeamONE.Agent.x64.msi” |
| ACCEPT\_THIRDPARTY\_LICENSES | 0/1 | Yes | Specifies if you want to accept the terms of the license agreement for the 3rd party components. Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_THIRDPARTY\_LICENSES="1" |
| ACCEPT\_EULA | 0/1 | Yes | Specifies if you want to accept the terms of the Veeam license agreement.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_EULA="1" |
| ACCEPT\_LICENSING\_POLICY | 0/1 | Yes | Specifies if you want to accept the terms of the Veeam licensing policy.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_LICENSING\_POLICY="1" |
| ACCEPT\_REQUIRED\_SOFTWARE | 0/1 | Yes | Specifies if you want to accept the terms of the required software license agreements.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_REQUIRED\_SOFTWARE="1" |
| INSTALLDIR | path | No | Installs the component to the specified location. By default, Veeam ONE uses the Veeam ONE Agent subfolder of the C:\Program Files\Veeam\Veeam ONE folder.  Example: INSTALLDIR="C:\Veeam\"  The component will be installed to the C:\Veeam\Veeam ONE Agent folder. |
| VO\_AGENT\_TYPE | 0/1 | Yes | Specifies the mode in which Veeam Analytics service will run. Specify 1 if you want to install Veeam Analytics service server. Specify 0 if you want to install Veeam Analytics service client.  Example: VO\_AGENT\_TYPE ="1" |
| VO\_AGENT\_SERVICE\_ACCOUNT\_NAME | user | Yes | Specifies a user account under which the Veeam ONE Agent service will run.  Example: VO\_AGENT\_SERVICE\_ACCOUNT\_NAME="ONESERVER\Administrator" |
| VO\_AGENT\_SERVICE\_ACCOUNT\_PASSWORD | password | Yes | This parameter must be used if you have specified the VO\_AGENT\_SERVICE\_ACCOUNT\_NAME parameter.  Specifies a password for the account that will be used to run Veeam ONE Agent.  Example: VO\_AGENT\_SERVICE\_ACCOUNT\_PASSWORD="p@ssw0rd" |
| VO\_BUNDLE\_INSTALLATION | 0/1 | Yes | This parameter must be used if you have specified 1 for the VO\_AGENT\_TYPE parameter.  Specify 1 to let Veeam ONE Monitor Service know about the installed Veeam ONE agent server. |
| VO\_AGENT\_SERVICE\_PORT | port | No | Specifies a port that will be used by Veeam ONE to communicate with Veeam ONE Agent. By default, port number 2805 is used.  Example: VO\_AGENT\_SERVICE\_PORT="2805" |

Example

Suppose you want to install Veeam ONE Client with the following configuration:

* Installation log location: C:\ProgramData\Veeam\Setup\Temp\Logs\AgentSetup.txt
* No user interaction
* Path to the MSI file: C:\Veeam\Monitor\VeeamONE.Agent.x64.msi

* Accept 3rd party license agreement
* Accept Veeam license agreement
* Accept required software license agreements
* Accept Veeam licensing policy

* Installation folder: default

* Agent mode: server
* Service user account: ONESERVER\Administrator
* Service user account password: p@ssw0rd
* Veeam ONE Agent communication port: default

The command to install Veeam ONE Agent with such configuration will have the following parameters:

|  |
| --- |
| msiexec.exe /L\*v "C:\ProgramData\Veeam\Setup\Temp\Logs\AgentSetup.txt" /qn /i "C:\Veeam\Monitor\VeeamONE.Agent.x64.msi" ACCEPT\_THIRDPARTY\_LICENSES="1" ACCEPT\_EULA="1" ACCEPT\_REQUIRED\_SOFTWARE="1" ACCEPT\_LICENSING\_POLICY="1" VO\_AGENT\_TYPE="1" VO\_BUNDLE\_INSTALLATION="1" VO\_AGENT\_SERVICE\_ACCOUNT\_NAME="ONESERVER\Administrator" VO\_AGENT\_SERVICE\_ACCOUNT\_PASSWORD="p@ssw0rd" |


