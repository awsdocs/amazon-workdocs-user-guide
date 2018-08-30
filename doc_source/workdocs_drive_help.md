# Using Amazon WorkDocs Drive<a name="workdocs_drive_help"></a>

For Windows users, Amazon WorkDocs Drive provides a native experience in Windows File Explorer for accessing all Amazon WorkDocs content\. With Amazon WorkDocs Drive, users get the power of the AWS Cloud on their desktops\. They can access all of their folders and files with minimal use of local storage\. Users don’t need to change the way they work, because they can see all of their folders and files in Windows File Explorer, which works just like the other files and folders on their desktop\.

Amazon WorkDocs Drive is available for Windows PC users and for Amazon WorkSpaces\. Amazon WorkDocs Drive can upload and download file sizes of up to 5 TB each, and allows file path lengths of up to 260 characters\.

**Topics**
+ [Installing Amazon WorkDocs Drive](#drive_install)
+ [Using Amazon WorkDocs Drive](#drive_use)
+ [Searching Amazon WorkDocs Drive](#drive_search)
+ [File Icons](#drive_icons)
+ [Enabling Offline Access and Syncing](#drive_offline)
+ [Troubleshooting Amazon WorkDocs Drive](#drive_troubleshoot)

## Installing Amazon WorkDocs Drive<a name="drive_install"></a>

If you have administrator privileges on your Windows device, you can install Amazon WorkDocs Drive\.

Amazon WorkDocs Drive is available only for 64\-bit versions of Windows 7, Windows 8, and Windows 10, Windows Server 2008, Windows Server 2012 R2, and Windows Server 2016\.

Amazon WorkDocs Drive requires Microsoft \.NET Framework 4\.6\.2 or newer, and HTTPS access on port 443 for all IP addresses for AWS\.

**To install Amazon WorkDocs Drive**

1. Download Amazon WorkDocs Drive from [https://amazonworkdocs\.com/en/clients](https://amazonworkdocs.com/en/clients)\.

1. Follow the installation prompts, including entering the name of your Amazon WorkDocs site\.

1. Your Amazon WorkDocs content appears as mounted drive W: on your computer\.

Administrators who are responsible for managing the domain\-joined machine fleet for their organization can install the Amazon WorkDocs Drive client by using Group Policy Objects \(GPO\) or System Center Configuration Manager \(SCCM\) Tools\.

**Note**  
When deploying with GPO or SCCM tools, we recommend installing the Amazon WorkDocs Drive client after users have logged in\.

The MSI installer for Amazon WorkDocs Drive supports an optional install parameter that pre\-populates the Amazon WorkDocs site information for users during registration; for example:

`SITEID` :*site\-name*

## Using Amazon WorkDocs Drive<a name="drive_use"></a>

You can access Amazon WorkDocs Drive from your Desktop shortcut\. It also appears as mounted drive W: in Windows File Explorer\.

You can perform operations directly from File Explorer, including creating, renaming, moving, and deleting files and folders\. Moving files and folders out of Amazon WorkDocs Drive moves them into your Amazon WorkDocs **Recycle bin**\.

**To work with files and folders**

1. Open File Explorer on your computer, and go to the W: drive\. 

1. Right\-click an Amazon WorkDocs file or folder, choose **Amazon WorkDocs Drive**, and choose one of the following actions:
   + To generate a link to share the content with other users, choose **Copy web link**\.
   + To view or edit the content in a web browser, choose **Open in browser**\.
   + To allow specific users in an organization to access the content, choose **Share by invite**\.
   + To mark a file or folder as a favorite, choose **Add to Favorites**\.
   + To prevent other users from changing the file while you’re working on it, choose **Lock**\. When you're done, choose **Unlock**\.

1. Your changes are automatically uploaded to Amazon WorkDocs and made available on all of your devices\.

## Searching Amazon WorkDocs Drive<a name="drive_search"></a>

Search for file names in Amazon WorkDocs Drive\.

**To search for content in Amazon WorkDocs Drive**

1. Choose the Amazon WorkDocs Drive icon in the system tray and left\-click to open the **Search** dialogue box\.

1. Enter search terms to search for files in Amazon WorkDocs\. Either search for files in all folders, or narrow your search to the `My Documents` or `Shared With Me` folders\.

1. Open the files directly from the search results list\.

## File Icons<a name="drive_icons"></a>

Amazon WorkDocs Drive provides the following visual icons to communicate file status:
+ **Blue arrow icon**—A file is syncing to the cloud\.
+ **Blue cloud icon**—A file is stored in the cloud\.
+ **Green checkmark icon**—A file is stored locally on your device\.
+ **Blue star icon**—A file or folder is marked as a Favorite\.

## Enabling Offline Access and Syncing<a name="drive_offline"></a>

Use Amazon WorkDocs Drive to sync favorite files and folders by enabling offline access\. 

**To enable offline access to files and folders**

1. In File Explorer, right\-click on a file or folder and choose **Amazon WorkDocs Drive**, **Add to Favorites**\.

1. Right\-click on the Amazon WorkDocs Drive icon in your Windows system tray\.

1. Choose **Keep Favorites on this Device**\.

Files or folders marked as favorites are synchronized between your **Favorites** on Amazon WorkDocs and the W: drive on your device\.

To turn off this option, choose **Remove Favorites from this Device**\.

You can also temporarily pause the syncing of Amazon WorkDocs content to your device, and resume syncing later\. If you have limited network bandwidth for syncing, you might consider using this option\.

**To pause file and folder syncing**

1. On your computer, right\-click on the Amazon WorkDocs Drive icon in your Windows system tray\.

1. Choose **Pause**\.

1. To resume syncing your files and folders, choose **Resume**\.

While syncing is paused, you can continue working on downloaded files that are available on your local device\. When syncing resumes, your changes are uploaded as new versions\.

## Troubleshooting Amazon WorkDocs Drive<a name="drive_troubleshoot"></a>

Troubleshooting tips for the most commonly encountered Amazon WorkDocs Drive errors are listed below\.

**Recovered Files**  
If you don’t have permissions to edit a file, you can't upload it to the Amazon WorkDocs site\. Your changes are saved in your local `Recovered files` folder, and you can upload the file to Amazon WorkDocs as a new file\.

**Report an Issue**  
Choose **Report an issue** from the Amazon WorkDocs Drive settings menu to provide a description of the problem and send logs\. This generates a tracking number, which you can include with the support case to help troubleshoot the issue\.