# Amazon WorkDocs Drive<a name="workdocs_drive_help"></a>

For Microsoft Windows users, Amazon WorkDocs Drive provides a native experience in Windows File Explorer for accessing all Amazon WorkDocs content\. With Amazon WorkDocs Drive, users get the power of AWS cloud on their desktops\. They can access all of their folders and files without using local storage\. Users don’t need to change the way they work, because they can see all of their folders and files in Windows File Explorer, which work just like the other files and folders on their desktop\.

Amazon WorkDocs Drive is available for all Amazon WorkSpaces customers and in limited preview for Windows PC users\.

The following currently aren't supported:

+ Multi\-user scenarios

+ 32\-bit client installer for Amazon WorkDocs Drive

+ Uploading or downloading a file size larger than 5 GB


+ [Installing Amazon WorkDocs Drive for Amazon WorkSpaces](#drive_install)
+ [Enrolling in the Limited Preview of Amazon WorkDocs Drive for PC](#drive_install-PC)
+ [Using Amazon WorkDocs Drive](#drive_use)
+ [Amazon WorkDocs Drive Options](#drive_options)
+ [File Icons](#drive_icons)

## Installing Amazon WorkDocs Drive for Amazon WorkSpaces<a name="drive_install"></a>

If you have administrator privileges, you can install Amazon WorkDocs Drive\.

Amazon WorkSpaces fleet administrators can install Amazon WorkDocs Drive for enterprise users by using group policy\.

**To install Amazon WorkDocs Drive**

1. Download Amazon WorkDocs Drive from [https://amazonworkdocs\.com/en/clients](https://amazonworkdocs.com/en/clients)\.

1. Follow the installation prompts, including entering the name of your Amazon WorkDocs site\.

1. Your Amazon WorkDocs content appears as mounted drive W: on your computer\.

## Enrolling in the Limited Preview of Amazon WorkDocs Drive for PC<a name="drive_install-PC"></a>

If you want to access a limited preview of this feature, go to [Amazon WorkDocs Preview](https://pages.awscloud.com/Amazon-WorkDocs-Preview.html)\.

After you are approved, you receive detailed instructions for downloading and installing Amazon WorkDocs Drive\.

## Using Amazon WorkDocs Drive<a name="drive_use"></a>

You can perform all the basic Amazon WorkDocs operations directly from File Explorer, including creating, renaming, moving, and deleting files and folders\.

**To work with files and folders**

1. Open File Explorer on your computer, and go to the W: drive\. 

1. Right\-click an Amazon WorkDocs file or folder, choose **Amazon WorkDocs Drive**, and choose one of the following actions:

   + To generate a link to share the content with other users, choose **Copy web link**\.

   + To view or edit the content in a web browser, choose **Open in browser**\.

   + To allow specific users in an organization to access the content, choose **Share by invite**\.

   + To mark a file or folder as a favorite, choose **Add to Favorites**\.

   + To prevent other users from making changes to the file while you’re working on it, choose **Lock**\. When you're done, choose **Unlock**\.

1. Your changes are automatically uploaded to Amazon WorkDocs and synced across all of your devices\.

To search for content in Amazon WorkDocs drive at any time, choose the Amazon WorkDocs drive icon in the system tray and left\-click to open the **Search** dialogue box\. Enter search terms to search for files in Amazon WorkDocs and open the files directly from Amazon WorkDocs on\-demand\.

## Amazon WorkDocs Drive Options<a name="drive_options"></a>

To access additional options for Amazon WorkDocs Drive, right\-click the W: drive, choose **Amazon WorkDocs Drive**, and choose one of the following:

+ **Open WorkDocs in browser**: Open Amazon WorkDocs in an internet browser\. 

+ **Store Favorites locally**: Save files and folders that are marked as Favorites on your local machine so you can access them while you’re offline\.

+ **View recovered files**: View files that can't be uploaded to the cloud due to conflicts\.

+ **Report an issue**: Report an issue about Amazon WorkDocs Drive\.

+ **Exit Drive**: Unmount Amazon WorkDocs Drive from the W: drive\.

## File Icons<a name="drive_icons"></a>

Amazon WorkDocs Drive provides the following visual icons to communicate file status:

+ **Blue arrow icon** indicates that a file is syncing to the cloud\.

+ **Blue cloud icon** indicates that a file is stored in the cloud\.

+ **Green checkmark icon** indicates that a file is stored locally\.

+ **Blue star icon** indicates that a file or folder is marked as a Favorite\.