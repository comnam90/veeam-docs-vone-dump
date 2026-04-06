---
title: "Monitoring Service"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/silent_install_monitor_srv.html"
last_updated: "9/2/2025"
product_version: "13.0.1.6168"
---

# Monitoring Service


To install Veeam ONE Monitoring service, use a command with the following syntax:

|  |
| --- |
| msiexec.exe [/L\*v "<path\_to\_log>"] /qn /i "<path\_to\_msi>" [ACCEPT\_THIRDPARTY\_LICENSES="1"][ACCEPT\_EULA="1"][ACCEPT\_REQUIRED\_SOFTWARE="1"][ACCEPT\_LICENSING\_POLICY="1"][VM\_MN\_SERVICEACCOUNT="<Veeam\_One\_Service\_Account>"][VM\_MN\_SERVICEPASSWORD="<Veeam\_One\_Service\_Account\_Password>"][VM\_MN\_SQL\_SERVER="<SQL\_server>"][VM\_MN\_SQL\_DATABASE="<database\_name>"] [VM\_MN\_SQL\_AUTHENTICATION="0"] [VM\_MN\_SQL\_USER="<SQL\_auth\_username>"] [VM\_MN\_SQL\_PASSWORD="<SQL\_auth\_password>"] [EDITLICFILEPATH="<path\_to\_license\_file>"] [VO\_LICENSE\_AUTOUPDATE="1"] [PF\_VEEAMONE="<path\_to\_installdir >"][VM\_GRPC\_SERVER\_PORT="<port\_number>"][VM\_MN\_CACHE="<path\_to\_cache\_folder>"] [VO\_INSTALLATION\_TYPE="0"] [VM\_MN\_SERVER\_AUTOUPDATE\_ENABLED="1"] |

The command has the following parameters:

Monitoring Service

| Option | Parameter | Required | Description |
| /L | \*v logfile | No | Creates an installation log file with the verbose output.  Specify an existing path to the log file as the parameter value. A setup log file created during the previous installation is cleared.  Example: /L\*v ”C:\ProgramData\Veeam\Setup\Temp\Logs\MonitorServerSetup.txt” |
| /q | n | Yes | Sets the user interface level to “no”, which means no user interaction is needed during installation. |
| /i | setup file | Yes | Installs Veeam ONE Monitoring service. Specify a full path to the setup file as the parameter value.  Example: /i “C:\Veeam\Monitor\VeeamONE.Monitor.Server.x64.msi” |
| ACCEPT\_THIRDPARTY\_LICENSES | 0/1 | Yes | Specifies if you want to accept the terms of the license agreement for the 3rd party components. Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_THIRDPARTY\_LICENSES="1" |
| ACCEPT\_EULA | 0/1 | Yes | Specifies if you want to accept the terms of the Veeam license agreement.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_EULA="1" |
| ACCEPT\_LICENSING\_POLICY | 0/1 | Yes | Specifies if you want to accept the terms of the Veeam licensing policy.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_LICENSING\_POLICY="1" |
| ACCEPT\_REQUIRED\_SOFTWARE | 0/1 | Yes | Specifies if you want to accept the terms of the required software license agreements.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_REQUIRED\_SOFTWARE="1" |
| VM\_MN\_SERVICEACCOUNT | user | Yes | Specifies a user account under which the Veeam ONE Services will run and that will be used to access Veeam ONE database in the Microsoft Windows authentication mode.  Example: VM\_MN\_SERVICEACCOUNT="ONESERVER\Administrator" |
| VM\_MN\_SERVICEPASSWORD | password | Yes | This parameter must be used if you have specified the VM\_MN\_SERVICEACCOUNT parameter.  Specifies a password for the account under which the Veeam ONE Services will run and that will be used to access Veeam ONE database.  Example: VM\_MN\_SERVICEPASSWORD="p@ssw0rd" |
| VM\_MN\_SQL\_SERVER | SQL server\instance | No | Specifies a Microsoft SQL server and instance on which the Veeam ONE database will be deployed. By default, Veeam ONE uses the LOCALHOST\VEEAMSQL2016 server.  Example: VM\_MN\_SQL\_SERVER="ONESERVER\VEEAMSQL2016\_MY" |
| VM\_MN\_SQL\_DATABASE | database | No | Specifies a name of the Veeam ONE database, by default, VeeamOne.  Example: VM\_MN\_SQL\_DATABASE="VeeamOneDB" |
| VM\_MN\_SQL\_AUTHENTICATION | 0/1 | No | Specifies if you want to use the Microsoft SQL Server authentication mode to connect to the Microsoft SQL Server where the Veeam ONE database is deployed. Specify 1 to use the SQL Server authentication mode. If you do not use this parameter, Veeam ONE will connect to the Microsoft SQL Server in the Microsoft Windows authentication mode (default value, 0).  Together with this parameter, you must specify the following parameters: VM\_MN\_SQL\_USER and VM\_MN\_SQL\_PASSWORD.  Example: VM\_MN\_SQL\_AUTHENTICATION="1" |
| VM\_MN\_SQL\_USER | user | No | This parameter must be used if you have specified the VM\_MN\_SQL\_AUTHENTICATION parameter.  Specifies a LoginID to connect to the Microsoft SQL Server in the SQL Server authentication mode.  Example: VM\_MN\_SQL\_USER="sa" |
| VM\_MN\_SQL\_PASSWORD | password | No | This parameter must be used if you have specified the VM\_MN\_SQL\_AUTHENTICATION parameter.  Specifies a password to connect to the Microsoft SQL Server in the SQL Server authentication mode.  Example: VM\_MN\_SQL\_PASSWORD="p@ssw0rd" |
| EDITLICFILEPATH | license path | No | Specifies a full path to the license file. If this parameter is not specified, Veeam ONE Community Edition will be installed.  Example: EDITLICFILEPATH="C:\Users\Administrator\Desktop\veeam\_one\_subscription\_100\_100.lic" |
| VO\_LICENSE\_AUTOUPDATE | 0/1 | No | Specifies if you want to enable automatic license update and usage reporting. By default, license auto update is enabled.  Example: VO\_LICENSE\_AUTOUPDATE="0" |
| PF\_VEEAMONE | path | No | Installs the component to the specified location. By default, Veeam ONE uses the Veeam ONE Monitor Server subfolder of the C:\Program Files\Veeam\Veeam ONE folder.  Example: PF\_VEEAMONE="C:\Veeam\"  The component will be installed to the C:\Veeam\Veeam ONE Monitor Server folder. |
| VM\_GRPC\_SERVER\_PORT | port number | No | Specifies the port number used for communication between Veeam ONE Monitoring service and Veeam ONE Web Client.  If you do not use this parameter, Veeam ONE Monotoring service will use the default port 2714.  Example: VM\_GRPC\_SERVER\_PORT="2714" |
| VM\_MN\_CACHE | path | No | Specifies a path to the folder where Performance Cache will be stored.  If you do not use this parameter, the performance cache will be stored to the C:\PerfCache folder (default).  Example: VM\_MN\_CACHE="D:\Veeam\PerfCache" |
| VO\_INSTALLATION\_TYPE | 0, 1 or 2 | No | Specifies the mode in which Veeam ONE will collect data from virtualization and Veeam Backup & Replication servers. Specify 1 to use the Veeam backup data and large-scale virtual infrastructure performance monitoring mode. Specify 2 to use the Veeam backup data only mode. If you do not use this parameter, Veeam ONE will collect data in the Veeam backup data and virtual infrastructure performance monitoring mode (default value, 0). For details, see [Choose Data Collection Mode](typical_choose_collection_mode.md).  Example: VO\_INSTALLATION\_TYPE="2" |
| VM\_MN\_SERVER\_AUTOUPDATE\_ENABLED | 0/1 | No | Specifies if you want to enable automatic updates after Veeam ONE installation. Specify 1 to enable automatic updates.  Example: VM\_MN\_SERVER\_AUTOUPDATE\_ENABLED="1" |

Example

Suppose you want to install Monitoring service with the following configuration:

* Installation log location: C:\ProgramData\Veeam\Setup\Temp\Logs\MonitorServerSetup.txt
* No user interaction
* Path to the MSI file: C:\Veeam\Monitor\VeeamONE.Monitor.Server.x64.msi
* Accept 3rd party license agreement
* Accept Veeam license agreement
* Accept required software license agreements
* Accept Veeam licensing policy
* Service user account: ONESERVER\Administrator
* Service user account password: p@ssw0rd
* License file location: C:\Users\Administrator\Desktop\veeam\_one\_subscription\_100\_100.lic
* Automatic license update: default
* Installation folder: default
* Path to Performance Cache folder: D:\Veeam\PerfCache
* SQL Server instance and database name: default
* Data collection mode: Veeam backup data and virtual infrastructure performance monitoring
* Automatic updates: enabled

The command to install Monitoring service with such configuration will have the following parameters:

|  |
| --- |
| msiexec.exe /L\*v "C:\ProgramData\Veeam\Setup\Temp\Logs\MonitorServerSetup.txt" /qn /i "C:\Veeam\Monitor\VeeamONE.Monitor.Server.x64.msi" ACCEPT\_THIRDPARTY\_LICENSES="1" ACCEPT\_EULA="1" ACCEPT\_REQUIRED\_SOFTWARE="1" ACCEPT\_LICENSING\_POLICY="1" VM\_MN\_SERVICEACCOUNT="ONESERVER\Administrator" VM\_MN\_SERVICEPASSWORD="p@ssw0rd" EDITLICFILEPATH="C:\Users\Administrator\Desktop\veeam\_one\_subscription\_100\_100.lic" VM\_MN\_CACHE="D:\Veeam\PerfCache" VO\_INSTALLATION\_TYPE="0" VM\_MN\_SERVER\_AUTOUPDATE\_ENABLED="1" |


