---
title: "Before You Begin"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/silent_mode_prerequisites.html"
last_updated: "11/13/2025"
product_version: "13.0.1.6168"
---

# Before You Begin


Before you start unattended installation, make sure that you perform the following steps:

1. Download the Veeam ONE installation image from the Veeam website. You can burn the downloaded image to a CD/DVD or mount the image to the target machine using disk image emulation software.
2. Check the system requirements. For details, see [System Requirements](system_requirements.md).
3. Log on to the target machine under the account that has the Local Administrator permissions on the machine. For details, see [Permissions](permissions.md).
4. Obtain a license file. If you do not specify a path to the license file during installation, Veeam ONE will operate in the Community Edition mode.
5. Define required and optional parameters in either the VoAnswerFile\_install.xml or VoClientAnswerFile\_install.xml file found in the \Setup\Silent\AnswerFiles folder of the Veeam ONE installation image:

* To install all Veeam ONE components use VoAnswerFile\_install.xml located in the /Setup/Silent/AnswerFiles/VO folder.

To upgrade or uninstall all Veeam ONE components, use the \_uninstall.xml and \_upgrade.xml files located in the same folder.

* To install Veeam ONE Client use VoClientAnswerFile\_install.xml located in the /Setup/Silent/AnswerFiles/VOClient folder.

To upgrade or uninstall Veeam ONE Client, use the \_uninstall.xml and \_upgrade.xml files located in the same folder.

Running Unattended Installation

To install Veeam ONE in unattended mode:

1. Open the product installation image file.
2. Navigate to the Setup\Silent\AnswerFiles folder.
3. Depending on what components you want to install, open VO for Veeam ONE or VOCLient for Veeam ONE Client.
4. In the relevant folder, open the VoAnswerFile\_install.xml file in your preferred text editor.

The file contains all the relevant information, including optional and required parameters for you to complete based on your installation requirements.

1. Once all parameters are complete, save the file and close.
2. Navigate back to the folder where the Veeam.Silent.Install.exe file exists (typically the setup\silent path of your root folder) and open the command line tool.
3. To check that all parameters are correct, run the Veeam.Silent.Install.exe /? command. This will display any unspecified parameters that must be completed before running unattended installation.
4. To run the install, enter Veeam.Silent.Install.exe /AnswerFile C:\YourDesiredLogFolderPath\_install.xml where YourDesireLogFolderPath is the installation log files location.

During installation the command line will return any error messages that need to be fixed.

|  |
| --- |
| Note: |
| You cannot use your Veeam account log in to verify your license, you can only specify the path to the license file. For details on [Step 4. Provide License](typical_provide_license.md). |


