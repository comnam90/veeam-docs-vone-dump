---
title: "Creating Veeam ONE Database with SQL Script"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/create_database_with_sql_script.html"
last_updated: "3/18/2025"
product_version: "13.0.1.6168"
---

# Creating Veeam ONE Database with SQL Script


In some circumstances, it might be undesired to create the Veeam ONE database automatically, using the Veeam ONE Setup wizard. For example, Veeam ONE components and the Microsoft SQL Server can be hosted on different systems, and you do not have sufficient permissions on the Microsoft SQL Server to create the database. In this case, you can use a SQL script to create the Veeam ONE database on a Microsoft SQL Server. The script is included with the Veeam ONE installation image.

To create the Veeam ONE database with the SQL script, perform the steps described below. Note that the database must be created before you start installation of Veeam ONE components.

Step 1. Locate the SQL Script

Download the Veeam ONE installation image and burn it to a blank CD/DVD or mount the image using disk image emulation software. If you are working with a virtual machine, use built-in tools of the virtualization management software to mount the installation image to the virtual machine.

In Windows Explorer, right-click the drive with the image, select Open and go to the <CD Drive>\Addins\SQLScript directory. Copy the VeeamONE.sql file to the location from which it can be accessed or run.

Step 2. Create the Veeam ONE Database

Connect to the necessary Microsoft SQL Server with Microsoft SQL Server Management Studio and create a new database (for example, VeeamOne).

Step 3. Run the SQL Script Against the Veeam ONE Database

Execute the VeeamONE.sql script against the Veeam ONE database in Microsoft SQL Server Management Studio.

Alternatively, you can execute the script using the sqlcmd utility. In the command prompt, run the command of the following form:

|  |
| --- |
| sqlcmd -S localhost\VEEAMSQL2017 -d VeeamOne -E -i “E:\Addins\SQLScript\VeeamONE.sql” |

The following command-line options are used to run the script:

Step 3. Run the SQL Script Against the Veeam ONE Database

| Option | Description |
| -S | Specifies the SQL Server instance to which sqlcmd connects. |
| -d | Specifies the name of the database against which the script is executed. |
| -E | Instructs sqlcmd to connect to the SQL Server Database Engine using Windows Integrated Security. |
| -i | Specifies the full path to the script file for execution. |

Step 4. Grant Database Permissions

Create a Microsoft SQL Server account with required permissions. For details, see [Connection to Microsoft SQL Server](connection_to_sql.md).


