---
title: "Reporting Service"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/silent_install_reporter_srv.html"
last_updated: "9/2/2025"
product_version: "13.0.1.6168"
---

# Reporting Service


To install Veeam ONE Reporting service, use a command with the following syntax:

|  |
| --- |
| msiexec.exe [/L\*v "<path\_to\_log>"] /qn /i "<path\_to\_msi>" [ACCEPT\_THIRDPARTY\_LICENSES="1"][ACCEPT\_EULA="1"][ACCEPT\_REQUIRED\_SOFTWARE="1"][ACCEPT\_LICENSING\_POLICY="1"][INSTALLDIR="<path\_to\_installdir >"][VO\_REPORTER\_SERVICE\_ACCOUNT\_NAME="<Veeam\_One\_Service\_Account>"][VO\_REPORTER\_SERVICE\_ACCOUNT\_PASSWORD="<Veeam\_One\_Service\_Account\_Password>"][VO\_REPORTER\_SQL\_SERVER\_NAME="<SQL\_server>"][VO\_REPORTER\_DATABASE\_NAME="<database\_name>"] [VO\_REPORTER\_AUTHENTICATION\_MODE="0"] [VO\_REPORTER\_SQL\_USER\_NAME="<SQL\_auth\_username>"] [VO\_REPORTER\_SQL\_PASSWORD="<SQL\_auth\_password>"] [EDITLICFILEPATH="<path\_to\_license\_file>"] [VO\_INSTALLATION\_TYPE="0"][VO\_REPORTER\_SERVER\_WEB\_API\_CERTIFICATE\_NAME="<certificate\_name>"]  [VO\_REPORTER\_SERVER\_COMMUNICATION\_PORT="<port\_number>"] [VO\_REPORTER\_SERVER\_WEB\_API\_PORT="<port\_number>"] |

The command has the following parameters:

Reporting Service

| Option | Parameter | Required | Description |
| /L | \*v logfile | No | Creates an installation log file with the verbose output.  Specify an existing path to the log file as the parameter value. A setup log file created during the previous installation is cleared.  Example: /L\*v ”C:\ProgramData\Veeam\Setup\Temp\Logs\ReporterServerSetup.txt” |
| /q | n | Yes | Sets the user interface level to “no”, which means no user interaction is needed during installation. |
| /i | setup file | Yes | Installs Veeam ONE Reporting Server. Specify a full path to the setup file as the parameter value.  Example: /i “C:\Veeam\Reporter\VeeamONE.Reporter.Server.x64.msi” |
| ACCEPT\_THIRDPARTY\_LICENSES | 0/1 | Yes | Specifies if you want to accept the terms of the license agreement for the 3rd party components. Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_THIRDPARTY\_LICENSES="1" |
| ACCEPT\_EULA | 0/1 | Yes | Specifies if you want to accept the terms of the Veeam license agreement.  Specify yes if you want to accept the terms and proceed with installation.  Example: ACCEPT\_EULA="1" |
| ACCEPT\_LICENSING\_POLICY | 0/1 | Yes | Specifies if you want to accept the terms of the Veeam licensing policy.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_LICENSING\_POLICY="1" |
| ACCEPT\_REQUIRED\_SOFTWARE | 0/1 | Yes | Specifies if you want to accept the terms of the required software license agreements.  Specify 1 if you want to accept the terms and proceed with installation.  Example: ACCEPT\_REQUIRED\_SOFTWARE="1" |
| INSTALLDIR | path | No | Installs the component to the specified location. By default, Veeam ONE uses the Veeam ONE Reporter Server subfolder of the C:\Program Files\Veeam\Veeam ONE folder.  Example: INSTALLDIR="C:\Veeam\"  The component will be installed to the C:\Veeam\Veeam ONE Reporter Server folder. |
| VO\_REPORTER\_SERVICE\_ACCOUNT\_NAME | user | Yes | Specifies a user account under which the Veeam ONE Services will run and that will be used to access Veeam ONE database in the Microsoft Windows authentication mode.  Example: VO\_REPORTER\_SERVICE\_ACCOUNT\_NAME="ONESERVER\Administrator" |
| VO\_REPORTER\_SERVICE\_ACCOUNT\_PASSWORD | password | Yes | This parameter must be used if you have specified the VO\_REPORTER\_SERVICE\_ACCOUNT\_NAME parameter.  Specifies a password for the account under which the Veeam ONE Services will run and that will be used to access Veeam ONE database.  Example: VO\_REPORTER\_SERVICE\_ACCOUNT\_PASSWORD="p@ssw0rd" |
| VO\_REPORTER\_SQL\_SERVER\_NAME | SQL server\instance | No | Specifies a Microsoft SQL server and instance on which the Veeam ONE database will be deployed. By default, Veeam ONE uses the LOCALHOST\VEEAMSQL2016 server.  Example: VO\_REPORTER\_SQL\_SERVER\_NAME="ONESERVER\VEEAMSQL2016\_MY" |
| VO\_REPORTER\_DATABASE\_NAME | database | No | Specifies a name of the Veeam ONE database, by default, VeeamOne.  Example: VO\_REPORTER\_DATABASE\_NAME="VeeamOneDB" |
| VO\_REPORTER\_AUTHENTICATION\_MODE\_NAME | 0/1 | No | Specifies if you want to use the Microsoft SQL Server authentication mode to connect to the Microsoft SQL Server where the Veeam ONE database is deployed. Specify 1 to use the SQL Server authentication mode. If you do not use this parameter, Veeam ONE will connect to the Microsoft SQL Server in the Microsoft Windows authentication mode (default value, 0).  Together with this parameter, you must specify the following parameters: VO\_REPORTER\_SQL\_USER\_NAME and VO\_REPORTER\_SQL\_PASSWORD.  Example: VO\_REPORTER\_AUTHENTICATION\_MODE\_NAME="1" |
| VO\_REPORTER\_SQL\_USER\_NAME | user | No | This parameter must be used if you have specified the VO\_REPORTER\_AUTHENTICATION\_TYPE\_NAME parameter.  Specifies a LoginID to connect to the Microsoft SQL Server in the SQL Server authentication mode.  Example: VO\_REPORTER\_SQL\_USER\_NAME="sa" |
| VO\_REPORTER\_SQL\_PASSWORD | password | No | This parameter must be used if you have specified the VO\_REPORTER\_AUTHENTICATION\_TYPE\_NAME parameter.  Specifies a password to connect to the Microsoft SQL Server in the SQL Server authentication mode.  Example: VO\_REPORTER\_SQL\_PASSWORD="p@ssw0rd" |
| EDITLICFILEPATH | license path | No | Specifies a full path to the license file. If this parameter is not specified, Veeam ONE Free Edition will be installed.  Example: EDITLICFILEPATH="C:\Users\Administrator\Desktop\veeam\_one\_subscription\_100\_100.lic" |
| VO\_REPORTER\_SERVER\_COMMUNICATION\_PORT | port number | No | Specifies the port number used for communication between Veeam ONE Reporting service and Veeam ONE Web Client.  If you do not use this parameter, Veeam ONE Reporting service will use the default port 2742.  Example: VO\_REPORTER\_SERVER\_COMMUNICATION\_PORT="2742" |
| VO\_REPORTER\_SERVER\_WEB\_API\_PORT | port number | No | Specifies the port number used for communication with Veeam ONE Web API.  If you do not use this parameter, Veeam ONE Reporting service will use the default port 2741.  Example: VO\_REPORTER\_SERVER\_WEB\_API\_PORT="2741" |
| VO\_REPORTER\_SERVER\_WEB\_API\_CERTIFICATE\_NAME | certificate name | No | Specifies the certificate to be used by Veeam ONE Web API. The certificate must be installed to the Certificate Store on the machine where you run installation.  If this parameter is not specified, a new self-signed certificate will be generated by openssl.exe. |
| VO\_INSTALLATION\_TYPE | 0, 1 or 2 | No | Specifies the mode in which Veeam ONE will collect data from virtualization and Veeam Backup & Replication servers. Specify 1 to use the Optimized for Advanced Scalability Deployment mode. Specify 2 to use The Backup Data Only mode. If you do not use this parameter, Veeam ONE will collect data in the Optimized for Typical Deployment mode (default value, 0). For details, see [Choose Data Collection Mode](typical_choose_collection_mode.md).  Example: VO\_INSTALLATION\_TYPE="2" |

Example

Suppose you want to install Veeam ONE Web Client server with the following configuration:

* Installation log location: C:\ProgramData\Veeam\Setup\Temp\Logs\ReporterServerSetup.txt
* No user interaction
* Path to the MSI file: C:\Veeam\Reporter\VeeamONE.Reporter.Server.x64.msi

* Accept 3rd party license agreement
* Accept Veeam license agreement
* Accept required software license agreements
* Accept Veeam licensing policy

* Installation folder: default

* Service user account: ONESERVER\Administrator
* Service user account password: p@ssw0rd
* SQL Server instance and database name: default

* License file location: C:\Users\Administrator\Desktop\veeam\_one\_subscription\_100\_100.lic

* Data collection mode: Optimized for Typical Deployment
* Communication port: default
* Web API port: default
* Web API certificate: generate new self-signed certificate

The command to install Veeam ONE Web Client server with such configuration will have the following parameters:

|  |
| --- |
| msiexec.exe /L\*v "C:\ProgramData\Veeam\Setup\Temp\Logs\ReporterServerSetup.txt" /qn /i "C:\Veeam\Reporter\VeeamONE.Reporter.Server.x64.msi" ACCEPT\_THIRDPARTY\_LICENSES="1" ACCEPT\_EULA="1" ACCEPT\_REQUIRED\_SOFTWARE="1" ACCEPT\_LICENSING\_POLICY="1" VO\_REPORTER\_SERVICE\_ACCOUNT\_NAME="ONESERVER\Administrator" VO\_REPORTER\_SERVICE\_ACCOUNT\_PASSWORD="p@ssw0rd" EDITLICFILEPATH="C:\Users\Administrator\Desktop\veeam\_one\_subscription\_100\_100.lic" VO\_INSTALLATION\_TYPE="0" |


