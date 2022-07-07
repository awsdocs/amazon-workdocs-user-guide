# Naming, uploading, and downloading files and folders<a name="client_add_files"></a>

The steps in this section explain the naming limitations for files and folders in Amazon WorkDocs, and how to upload and download files and folders\. If you have a Windows machine, you can use Amazon WorkDocs Companion with File Explorer to upload multiple files and folders\. For more information, see [Using Amazon WorkDocs Companion](companion.md)\.

## Naming limitations<a name="naming"></a>

You can make several mistakes when naming files and folders in Amazon WorkDocs\. Here's a list of what to look for and avoid\.

**Important**  
Pay special attention to these conventions if you're migrating files\. Incorrect file and folder names can break the migration process\. For more about migration, see [Preparing for migration](https://docs.aws.amazon.com/workdocs/latest/adminguide/prepare.html)\.
+ **File names** – Must be 255 characters or less\.
+ **Folder paths** – Amazon WorkDocs only displays the first 260 characters of a folder path\. 
+ **Trailing spaces** – For example: an extra space at the end of a file name\.
+ **Periods at the beginning or end** – For example: `.file`, `.file.ppt`, `.`, `..`, or `file.`
+ **Tildes at the beginning or end** – For example: `file.doc~`, `~file.doc`, or `~$file.doc`
+ **File names ending in `.tmp`** – For example: `file.tmp`
+ **File names exactly matching these case\-sensitive terms** – `Microsoft User Data`, `Outlook files`, `Thumbs.db`, or `Thumbnails`
+ **File names containing any of these characters** – `*` \(asterisk\), `/` \(forward slash\), `\` \(back slash\), `:` \(colon\), `<` \(less than\), `>` \(greater than\), `?` \(question mark\), `|` \(vertical bar/pipe\), `"` \(double quotes\), or `\202E` \(character code 202E\)\.

## Uploading files<a name="upload-files"></a>

**To upload files or a folder**

1. In the web client, choose **Upload**, **Upload files** or **Upload folder**\.

1. Select the check boxes next to the files or folders that you want to upload\. 

You can also add files by dragging and dropping them from your computer to the web client\. But remember that not all browsers support file drag\-and\-drop\.

**To upload a new version of a file**

1. In the web client, open the file\.

1. For **Actions**, choose **Upload new version** and select the version of the file to upload\.

## Downloading files<a name="download-files"></a>

You can also download files or folders from the web client\. 

**To download files or folders**  
In the web client, do one of the following:
+ Select the one or more check boxes next to the files or folders that you want to download, open the **Actions** menu and choose **Download**\.
+ Open the file, then open the **Actions** menu and choose **Download**\.
+ Open the folder\. The folder name appears in a list, with a downward facing arrow\. Open that list and choose **Download**\.

**Note**  
On a PC, files and folders land in these locations by default:  
Individual files land in **Downloads**\.
Multiple files land in a **Downloads/WorkDocsDownloads/WorkDocs\-Bulk\-Download\-***mm\-dd\-yyyy* folder\.
Folders land in a **Downloads/WorkDocsDownloads/***folder name* folder\.
On a Macintosh, downloaded files land by default in the *Hard Drive Name***/Users/***User Name***/WorkDocsDownloads** folder\.