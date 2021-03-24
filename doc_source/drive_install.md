# Installing Amazon WorkDocs Drive<a name="drive_install"></a>

You must be an administrator on your device to install Amazon WorkDocs Drive\.

Amazon WorkDocs Drive is available for 64\-bit versions of Windows 7, Windows 8, and Windows 10, plus Windows Server 2008 R2 SP1, Windows Server 2012 R2, and Windows Server 2016\.

Amazon WorkDocs Drive for Windows also requires Microsoft \.NET Framework 4\.6\.2 or later\. You can download the latest framework from [ https://dotnet\.microsoft\.com/download/dotnet\-framework](https://dotnet.microsoft.com/download/dotnet-framework)\.

Amazon WorkDocs Drive is available for macOS version 10\.11 or later\.

Amazon WorkDocs Drive isn’t supported on Apple silicon products\.

**To install Amazon WorkDocs Drive on the supported platforms**

1. Download Amazon WorkDocs Drive from [ https://amazonworkdocs\.com/en/clients ](https://amazonworkdocs.com/en/clients) and follow the installation prompts\.

1. Open Amazon WorkDocs Drive\. When prompted, enter the name of your Amazon WorkDocs site, user name, and password\.

**Note**  
macOS High Sierra 10\.13 users might encounter this error message during installation: `System Extension Blocked`\.  
To unblock the installation, open **System Preferences**, choose **Security & Privacy**, then choose **Allow**\.

**To install Amazon WorkDocs Drive for macOS Big Sur on Intel machines**

1. Complete the steps in the previous section, and then choose the Amazon WorkDocs Drive icon on the menu bar\.

1. In the Amazon WorkDocs Drive window, choose **Open Drive in Finder**, and when prompted to update the system extension, choose **Open Security Preference**\.

1. In the **Security Preferences** window, choose the lock icon, enter your credentials, and choose **Allow** for **System software from developer "AMZN Mobile LLC" has been updated\.** 

1. Restart the machine\.

1. Open terminal\. If you don't know how to do that, search for "terminal" in Finder\.

1. In your terminal, enter **kextstat \| grep fuse** and press **Enter**\.

1. Repeat the previous step to run these commands in the order listed: **clear**, **exist**\. Close The terminal window when finished\.