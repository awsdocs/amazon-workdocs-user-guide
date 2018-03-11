# Amazon WorkDocs Sync Client<a name="sync_client_help"></a>

Amazon WorkDocs provides a client synchronization application that allows you to synchronize a folder on your desktop with the Amazon WorkDocs service\. The local Amazon WorkDocs folder is a mirror of your Amazon WorkDocs `My documents` and `Shared with me` folders and subfolders in the cloud\. If you add a file under your local Amazon WorkDocs folder, that file is automatically synchronized to your online Amazon WorkDocs `My documents` folder, in the background\. Likewise, if you delete a file from your online Amazon WorkDocs `My documents` folder or one of its subfolders, the file is automatically removed from your local Amazon WorkDocs folder\. This provides you with safe and secure off\-site storage for your important files\.

You can store any type of file in Amazon WorkDocs, except for those defined in [Excluded Files and Folders](#sync_excluded_files)\. The Amazon WorkDocs collaboration clients can display previews for many different types of files, depending on the internet media type of the file\. Support for additional media types is constantly being added\.

**Note**  
It can take up to a few minutes for syncing to begin, depending on your connection speed, bandwidth availability, and the size of the files you are syncing\.


+ [System Requirements](#sync_sys_reqs)
+ [Installing the Sync Application](#sync_install)
+ [Setting up the Sync Application](#sync-set-up)
+ [Single Sign\-On](#sync_sso)
+ [Changing the Amazon WorkDocs Account](#sync_changeaccount)
+ [Excluded Files and Folders](#sync_excluded_files)
+ [Sync Operation](#sync_operation)
+ [Using the Shared Sync Folder](#sync_shared_folder)
+ [Deleting Shared Folders and Files](#delete_shared)
+ [Selecting a Sync Folder](#sync_select_folders)
+ [Uninstalling the Sync Application](#sync-uninstall)
+ [Troubleshooting Sync Issues](#sync_troubleshooting)

## System Requirements<a name="sync_sys_reqs"></a>

The Amazon WorkDocs sync application requires a computer running one of the following operating systems:

+ Microsoft Windows 7, Windows 8, or Windows 10

+ Microsoft Windows Server 2008

+ Microsoft Windows Server 2012 R2 \(with Microsoft AD, not Simple AD\)

+ macOS 10\.10 or later

On all Windows clients, including all WorkSpaces, you must enable JavaScript in Internet Explorer\. For more information, see [How to enable JavaScript in a web browser?](http://support.microsoft.com/gp/howtoscript)\.

The sync application requires HTTPS access on port 443 for all IP addresses for AWS\.

The sync application communicates with the Java engine\. You can identify the port as follows:

+ On Windows, locate the client\.log file in the `%USERPROFILE%\AppData\Local\Amazon WorkDocs\SyncClient` folder\. Search for `http://127.0.0.1`\. The port is specified as follows: `http://127.0.0.1:port`\.

+ On macOS, locate the sync\-service\.port file in the `/Users/user/Library/Application Support/Amazon WorkDocs/SyncClient` folder\. The port is stored in plaintext\.

The sync application supports local drives, but does not support non\-local drives, including network drives and external USB drives\. 

## Installing the Sync Application<a name="sync_install"></a>

The Amazon WorkDocs sync application is available for both Windows and macOS desktops\.

**To download and install the Amazon WorkDocs sync application using the console**

1. Connect to the Amazon WorkDocs console

1. In the navigation menu, choose **Install sync client**\.  
![\[Amazon WorkDocs console navigation\]](http://docs.aws.amazon.com/workdocs/latest/userguide/images/webapp_install_syncclient.png)

1. From the list of available installation options, choose an option and complete the installation\.

**To download and install the Amazon WorkDocs sync application for Windows**

1. Download the Amazon WorkDocs sync application installer for Windows from [https://d28gdqadgmua23\.cloudfront\.net/win/AmazonWorkDocsSetup\.exe](https://d28gdqadgmua23.cloudfront.net/win/AmazonWorkDocsSetup.exe)\.

1. Run the installer\. The Amazon WorkDocs sync application is downloaded, installed, and launched\.

**To download and install the Amazon WorkDocs sync application for macOS**

1. Open the Amazon WorkDocs sync application for macOS from [https://d28gdqadgmua23\.cloudfront\.net/mac/Amazon WorkDocs\.pkg](https://d28gdqadgmua23.cloudfront.net/mac/Amazon WorkDocs.pkg)\.

1. Drag the Amazon WorkDocs Sync icon to the **Applications** folder\. 

1. Open the **Applications** folder and open **Amazon WorkDocs Sync**\.

## Setting up the Sync Application<a name="sync-set-up"></a>

The next step is registering the Amazon WorkDocs sync application\. You can run the Amazon WorkDocs sync application on more than one local desktop\. No matter how many desktops you synchronize, all of the files and folders in the sync folder are replicated on all of the desktops\.

**To complete the initial setup of the Amazon WorkDocs sync application**

1. In the **Amazon WorkDocs Setup** dialog box, choose **Get Started**\. 

1. Type your Amazon WorkDocs site URL, which is provided by your Amazon WorkDocs administrator and choose **Next**\.

1. Type your Amazon WorkDocs user credentials and choose **Sign In**\.

1. The default for the sync folder is the `WorkDocs` folder in your user directory\. This folder is created if it does not already exist\. To choose a different folder, choose **Change** and select the folder\. Choose **Next**\.
**Note**  
If you have previously installed the Amazon WorkDocs sync client, the initial folder may be renamed\. We recommend using the default name to ensure that previous content is not overwritten\.

1. Select the option to synchronize all files and folders or the option to synchronize only selected folders, and then choose **Next**\.

1. Choose **Ok** to exit the setup program\.

**Note**  
The Amazon WorkDocs sync client is updated automatically when new versions are available\.

## Single Sign\-On<a name="sync_sso"></a>

The Amazon WorkDocs sync application does not require additional steps to enable single sign\-on\. If you experience any issues, restart the sync application to have the settings applied on your behalf\.

## Changing the Amazon WorkDocs Account<a name="sync_changeaccount"></a>

To change the Amazon WorkDocs account you have registered within the sync client, do the following:

**Changing the Amazon WorkDocs account used in the sync client**

1. Open the context \(right\-click\) menu for the Amazon WorkDocs icon in your taskbar \(or menu bar if you have a macOS\)\.

1. Choose the gear icon to open **Preferences** and choose **Deregister this account**\. Confirm your selection\.

1. To register a new site, choose **Get Started** and go through the site registration steps\.

## Excluded Files and Folders<a name="sync_excluded_files"></a>

Any files or folders that meet the following criteria are not synchronized:

+ Any file or folder name that starts with a period \(\.\), such as the following: 

  + "`.lock`"

  + "`.~doctor.ppt`"

  + "`.`"

  + "`..`"

+ Any file or folder name that starts or ends with a tilde \(\~\), such as the following:

  + "`hello.txt~`"

  + "`~WRD0000.tmp`"

  + "`.~doctor.ppt`"

  + "`~$filename.txt`"

+ Any file or folder name ending with "`.tmp`", such as the following:

  + "`pptC407.tmp`"

  + "`~WRD0000.tmp`"

+ Any file or folder with one of the following names \(the name and case must be an exact match\):

  + `Microsoft User Data`

  + `Outlook Files`

  + `Thumbs.db`

  + `Thumbnails`

  + `thumbnails`

+ Any file or folder name that includes any of the following characters:

  + \* \(asterisk\)

  + / \(forward slash\)

  + \\ \(back slash\)

  + : \(colon\)

  + < \(less than\)

  + > \(greater than\)

  + ? \(question mark\)

  + | \(vertical bar/pipe\)

  + " \(double quotes\)

  + character code 202E \(\\202E\)

+ Any file/folder that has a trailing space \(‘ ‘\) or period \(‘\.’\) character: 

  + `"filename "`

  + `"filename."`

+ Any file or folder name that is longer than 255 characters

+ Any file that is greater than 5 TB

## Sync Operation<a name="sync_operation"></a>

After the Amazon WorkDocs sync application is installed and running, any non\-excluded files in your local sync folder that you add, remove, or modify are automatically synchronized with your Amazon WorkDocs `My documents` folder\.

**Note**  
Moving files you own out of the sync folder deletes them from your Amazon WorkDocs file repository in the web client, mobile apps, and other devices where the Amazon WorkDocs sync client is installed\.

File uploads and downloads that are in progress when you close the sync application are automatically resumed the next time you log in\.

You can add, remove, or modify files while offline and these changes will be updated to your Amazon WorkDocs repository when the sync client connects the next time\.

To see the upload and sync status of your files, choose the Amazon WorkDocs icon in the status notification tray on your computer\. You also see a list of recently synced files as well as when it was synced\.

## Using the Shared Sync Folder<a name="sync_shared_folder"></a>

In addition to the files and folders that you own, the Amazon WorkDocs sync application also allows you to sync the files and folders that have been shared with you\. 

**To sync files and folders that have been shared with you**

1. Open the preferences dialog box for the Amazon WorkDocs sync application\.

1. Choose **Enable Shared Folder Sync**, and then close the preferences dialog box\.

A folder called **Shared With Me** is created in your Amazon WorkDocs sync folder that contains copies of all of the files and folders that have been shared with you\.

## Deleting Shared Folders and Files<a name="delete_shared"></a>

To free up local storage space, you can delete a file or folder that has been shared with you in the **Shared with me** folder\. There are two ways to do this, depending on where you want the file or folder deleted from\.

To delete a file or folder from your desktop, but still allow it to be accessed in the **Shared with me** folder by other users, other devices, and the web client, delete it only from your computer\. You can access it again from the **Shared with me** folder by re\-selecting it from the **WorkDocs Selective Sync Settings** on your desktop\. 

If you permanently delete a file or folder in the **Shared with me folder** for all users, all of your devices, and the web client, it cannot be accessed again\. You must have collaborator or co\-owner permissions to do this\. 

**To delete a file or folder from your computer only**

+ Delete it from the **Shared with me** folder on your desktop, or de\-select it from the **WorkDocs Selective Sync Settings** on your desktop\.

**To delete a file or folder for all users and devices**

1. Open the web client\.

1. On the **Shared with me** tab, choose the file or folder to delete\.

1. Choose **Delete**\. 

1. The file or folder appears in the **Recycle Bin** of your web client\.

   + To restore the item, open the context \(right\-click\) menu of the **Recycle Bin**, choose **Open**, right\-click on the item, and choose **Restore**\.

   + To delete the item permanently, open the context \(right\-click\) menu of the **Recycle Bin** and choose **Empty Recycle Bin**\.
**Note**  
If you delete a file or folder from `My documents`, it is moved to the recycle bin on the web client\. It does not appear on the sync client folders on any other device for you or other users\.

## Selecting a Sync Folder<a name="sync_select_folders"></a>

Syncing files and folders automatically backs up your local data to Amazon WorkDocs\. You can sync all files and folders or choose specific files or folders, which allows you to avoid syncing large amounts of data unnecessarily\. Keep the following notes in mind when selecting a folder:

+ You can only sync files that are included in your Amazon WorkDocs sync folder\. Amazon WorkDocs sync does not support selecting folder outside of the Amazon WorkDocs sync folder\.

+ If the Amazon WorkDocs sync client is registered to a folder that includes files, they are updated as the latest versions of the files\. To avoid overwriting online files with files synced from your desktop, select a new empty folder as your Amazon WorkDocs sync folder\.

To remove files and folders from your computer, de\-select them in **WorkDocs Selective Sync Settings**\. This removes them from your computer, but they remain available for other users\. You can still access them from the web client and your other computers\.

**To select sync folders during setup**

1. Begin the Amazon WorkDocs setup process\.

1. When you are prompted to choose files to sync, choose **Sync only the files and folders I select from WorkDocs** or **Sync all file and folders from WorkDocs**\.

**To sync specific files or folders after setup**

1. Open the context \(right\-click\) menu for the Amazon WorkDocs icon in your taskbar \(or menu bar if you use macOS\)\.

1. Choose the gear icon to open **Preferences** and choose **Select files and folders to sync**\.

1. Select the check boxes for the items to sync\. You can expand the top\-level folders to select subfolders and individual documents\.

1. To sync all new folders and files that you create in the future, choose **My Documents**, **New Folders And Files**, **Update**\.

## Uninstalling the Sync Application<a name="sync-uninstall"></a>

You can uninstall the Amazon WorkDocs sync application from your local device without affecting the files that were last synchronized to or from your sync folder\. These files and folders are no longer automatically updated after you uninstall the sync client, and you can delete them at any time\.

**To uninstall the Amazon WorkDocs sync application for Windows**

1. In Control Panel, choose **Programs and Features**, **Amazon WorkDocs**, **Uninstall**\.

1. When prompted for confirmation, choose **OK**\.

1. \(Optional\) Delete the files from your sync folder\.

**To uninstall the Amazon WorkDocs sync application for macOS**

1. Open the context menu for the Amazon WorkDocs icon in your menu bar\.

1. Choose the gear icon to open **Preferences** and choose **Quit WorkDocs**\.

1. Open the **Applications** folder\.

1. Drag the Amazon WorkDocs icon to the trash\.

1. Empty the trash\.

1. \(Optional\) Delete the files from your sync folder\.

## Troubleshooting Sync Issues<a name="sync_troubleshooting"></a>

The following are common issues and fixes with the Amazon WorkDocs sync client\. For further assistance, you can [contact Support](http://docs.aws.amazon.com/awssupport/latest/user/getting-started.html) or post on the [AWS forum](https://aws.amazon.com/workdocs/resources/#forum)\.


+ [Files Are Not Syncing](#sync_errors)
+ [Obtaining the Amazon WorkDocs Sync Client Log File](#sync_logs)

### Files Are Not Syncing<a name="sync_errors"></a>

If your files are not syncing, you can check for the following issues:

+ Excluded files in the sync folder\. For more information about file naming restrictions, see [Excluded Files and Folders](#sync_excluded_files)\.

+ File naming collisions\. Ensure that each file name is unique\.

+ Selective sync preventing sync\. Verify your selective sync settings and ensure that your folder is selected\.

+ Internet connectivity issues\. Syncing resumes after internet connectivity is resumed\.

### Obtaining the Amazon WorkDocs Sync Client Log File<a name="sync_logs"></a>

To further troubleshoot issues with the Amazon WorkDocs sync client, you may be asked to provide your Sync activity logs to help investigate and resolve your issue\. You can do so with the following steps:

**Obtaining the Amazon WorkDocs sync client log files**

1. Open the context \(right\-click\) menu for the Amazon WorkDocs icon in your taskbar \(or menu bar if you use macOS\)\.

1. Choose the gear icon to open **Preferences** and choose **Send Diagnostic Logs**\.

1. In the description field, include the following information:

   + Short description of the problem

   + Full path of the affected documents or folders

   + Names of affected users

1. Choose **Submit**\.