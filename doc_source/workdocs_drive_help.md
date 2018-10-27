# Using Amazon WorkDocs Drive<a name="workdocs_drive_help"></a>

Amazon WorkDocs Drive provides a native desktop experience for accessing Amazon WorkDocs content\. With Amazon WorkDocs Drive, users get the power of the AWS Cloud on their desktops\. They can access all of their folders and files with minimal use of local storage\. Users don’t need to change the way they work, because they can see all of their Amazon WorkDocs folders and files on their computer\.

Amazon WorkDocs Drive is available for PC and macOS users, and for Amazon WorkSpaces\. Amazon WorkDocs Drive can upload and download file sizes of up to 5 TB each, and allows file path lengths of up to 260 characters\.

**Topics**
+ [Installing Amazon WorkDocs Drive](#drive_install)
+ [Using Amazon WorkDocs Drive](#drive_use)
+ [Searching Amazon WorkDocs Drive](#drive_search)
+ [File Icons](#drive_icons)
+ [Enabling Offline Access and Syncing](#drive_offline)
+ [Troubleshooting Amazon WorkDocs Drive](#drive_troubleshoot)

## Installing Amazon WorkDocs Drive<a name="drive_install"></a>

If you have administrator permissions on your device, you can install Amazon WorkDocs Drive\.

Amazon WorkDocs Drive is available for 64\-bit versions of Windows 7, Windows 8, and Windows 10, and Windows Server 2008, Windows Server 2012 R2, and Windows Server 2016\. Amazon WorkDocs Drive for Windows also requires Microsoft \.NET Framework 4\.6\.2 or later\. Amazon WorkDocs Drive is available for macOS version 10\.11 or later\.

Amazon WorkDocs Drive requires HTTPS access on port 443 for all IP addresses for AWS\. 

**To install Amazon WorkDocs Drive**

1. Download Amazon WorkDocs Drive from [Amazon WorkDocs Resources](https://aws.amazon.com/workdocs/resources/) and follow the installation prompts\.

1. Open Amazon WorkDocs Drive\. When prompted, enter the name of your Amazon WorkDocs site, username, and password\.

**Note**  
macOS High Sierra 10\.13 users might encounter this error message during installation: `System Extension Blocked`\. To unblock the installation, open **System Preferences** on your computer and choose **Security & Privacy**\. Then, choose **Allow** to install Amazon WorkDocs Drive\.

### Installing Amazon WorkDocs Drive for Windows to Multiple PCs and WorkSpaces<a name="install-multiple"></a>

Administrators who are responsible for managing the domain\-joined machine fleet for their organization can install the Amazon WorkDocs Drive client by using Group Policy Objects \(GPO\) or System Center Configuration Manager \(SCCM\) Tools\.

**Note**  
When deploying with GPO or SCCM tools, we recommend installing the Amazon WorkDocs Drive client after users have logged in\.

The MSI installer for Amazon WorkDocs Drive supports an optional install parameter that pre\-populates the Amazon WorkDocs site information for users during registration; for example:

`SITEID` :*site\-name*

### Mounting Amazon WorkDocs Drive for macOS Using the Windows Subsystem for Linux<a name="mount-linux"></a>

You can mount Amazon WorkDocs Drive for macOS using the following commands in the Windows Subsystem for Linux\. For more information, see [File System Improvements to the Windows Subsystem for Linux](https://blogs.msdn.microsoft.com/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)\.

```
              $ sudo mkdir /mnt/w
              $ sudo mount -t drvfs W: /mnt/w
              $ cd /mnt/w
              $ ls
```

## Using Amazon WorkDocs Drive<a name="drive_use"></a>

Windows users can open Amazon WorkDocs Drive from the **Desktop** shortcut or the W: drive in File Explorer\. macOS users can open Amazon WorkDocs Drive from the menu bar or from the Finder under **Favorites**\.

Create, rename, move, and delete files and folders directly from Amazon WorkDocs Drive on your computer\. Moving files out of Amazon WorkDocs Drive deletes them\. Deleted files are moved to your **Recycle bin** on Amazon WorkDocs\.

**Note**  
If two files or folders have the same name, only one of them appears in Amazon WorkDocs Drive\.

**To work with files and folders**

1. 

   Do one of the following:  
**Windows**  
Open Amazon WorkDocs Drive from File Explorer, or choose or right\-click the Amazon WorkDocs Drive icon in the notification area and choose **Open Drive**\.  
**macOS**  
Open Amazon WorkDocs Drive from the Finder, under **Favorites**, or choose or right\-click the Amazon WorkDocs Drive icon on the menu bar and choose **Open Drive**\.

1. Choose or right\-click an Amazon WorkDocs file or folder, choose **Amazon WorkDocs Drive**, and choose one of the following actions:
   + To generate a link to share the content with other users, choose **Copy web link**\.
   + To view or edit the content in a web browser, choose **Open in browser**\.
   + To mark a file or folder as a favorite, choose **Add to Favorites**\.

   The following actions apply to files only:
   + To allow specific users in an organization to access the content, choose **Share by invite**\.
   + To prevent other users from changing the file while you're working on it, choose **Lock and Edit**\. When you're done, choose **Unlock**\.

1. Your changes are automatically uploaded to Amazon WorkDocs and made available on all of your devices\.

To quit running Amazon WorkDocs Drive on your device, do the following\.

**To quit Amazon WorkDocs Drive**
+ Choose or right\-click the Amazon WorkDocs Drive icon in the notification area or menu bar, and choose **Quit**\.

To uninstall Amazon WorkDocs Drive from your device, do the following\.

**To uninstall Amazon WorkDocs Drive**

1. Choose or right\-click the Amazon WorkDocs Drive icon in the notification area or menu bar, and choose **Quit**\.

1. 

   Do one of the following:  
**Windows**  
From the **Control Panel**, choose **Programs and Features**, **Amazon WorkDocs Drive**, **Uninstall**, **OK**\.  
**macOS**  
From the **Applications** folder, choose or right\-click the Amazon WorkDocs Drive icon, then choose **Move to Trash**\.

## Searching Amazon WorkDocs Drive<a name="drive_search"></a>

Search for file names in Amazon WorkDocs Drive\. 

**To search for content in Amazon WorkDocs Drive**

1. Choose or right\-click the Amazon WorkDocs Drive icon in the notification area or menu bar, then choose **Search**\.

1. Enter search terms to search for files in Amazon WorkDocs\. File names are case sensitive\. Either search for files in all folders, or narrow your search to the `My Documents` or `Shared With Me` folders\.

1. Open the files directly from the search results list\.

**Note**  
File Explorer search for Windows and Spotlight search for macOS are not supported in Amazon WorkDocs Drive\.

## File Icons<a name="drive_icons"></a>

Amazon WorkDocs Drive provides the following visual icons to communicate file status:
+ **Gray arrow icon**—A file is syncing to the cloud\.
+ **Blue cloud icon**—A file is stored in the cloud\.
+ **Green checkmark icon**—A file is stored locally on your device\.
+ **Blue star icon**—A file or folder is marked as a Favorite\.
+ **Red lock icon**—A file is locked by the user for exclusive editing\.

## Enabling Offline Access and Syncing<a name="drive_offline"></a>

Enable offline access to your files and folders so that you can work on your content when your device is offline\. Changes made in Amazon WorkDocs Drive while offline will sync to the Amazon WorkDocs website the next time your device is online\.

To enable offline access to files and folders, first add them to your **Favorites**, then enable the option to store **Favorites** for offline use\.

**To enable offline access to files and folders**

1. 

   Do one of the following:  
**Windows**  
Open File Explorer on your computer, and go to the W: drive\.   
**macOS**  
Open the Finder on your computer, and go to Amazon WorkDocs Drive under **Favorites**\.

1. Choose or right\-click the files or folders that you want access offline, and choose **Amazon WorkDocs Drive**, **Add to Favorites**\.

1. In the notification area or menu bar, choose or right\-click the Amazon WorkDocs Drive icon, and select **Store Favorites for offline use**\.

1. Wait for Amazon WorkDocs Drive to finish downloading favorited content from the Amazon WorkDocs website to your device\. This can take some time depending on how much content is downloaded\.

To turn off this option and remove the downloaded content from your device, choose or right\-click the Amazon WorkDocs Drive icon in your notification area or menu bar, and clear **Store Favorites for offline use**\.

You can temporarily pause the syncing of Amazon WorkDocs content to your device, and resume syncing later\. If you have limited network bandwidth for syncing, you might consider using this option\.

**To pause file and folder syncing**

1. In the notification area or menu bar, choose or right\-click the Amazon WorkDocs Drive icon\.

1. Select **Pause sync**\.

1. To resume syncing your files and folders, clear **Pause sync**\.

While syncing is paused, you can continue working on downloaded files that are available on your local device\. When syncing resumes, your changes are uploaded as new versions\.

## Troubleshooting Amazon WorkDocs Drive<a name="drive_troubleshoot"></a>

Troubleshooting tips for the most commonly encountered Amazon WorkDocs Drive errors are listed below\.

**Recovered Files**  
If you don't have permissions to edit a file, you can't upload it to the Amazon WorkDocs site\. Your changes are saved in your local `Recovered files` folder, which you can open from the Amazon WorkDocs Drive menu by choosing **Help**, **Recovered files**\. From there, you can upload the file to Amazon WorkDocs as a new file\.

**Report an Issue**  
From the Amazon WorkDocs Drive menu, choose **Help**, **Report an issue** to send us a description of the problem\. Take note of the tracking number provided, which serves as a reference for support cases or correspondence with us\.

**Known Limitations**  
Symlinks are not supported\.