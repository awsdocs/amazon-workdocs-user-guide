# Troubleshooting Amazon WorkDocs Drive<a name="drive_troubleshoot"></a>

The following sections provides troubleshooting tips for common Amazon WorkDocs Drive errors\. Choose a section to expand it\.

## Critical Dependency Unavailable<a name="ts-1"></a><a name="critical"></a>

Restart the **Message Queuing** service on your computer by opening the **Services** app\. For **Message Queuing**, choose **Restart** or **Start**\.

If the error persists, open **Computer Management**, **Services and Applications**\. If **Message Queuing** does not appear in the navigation pane, [uninstall **Message Queuing**](https://docs.particular.net/transports/msmq/uninstalling-msmq) and Amazon WorkDocs Drive\. When you reinstall Amazon WorkDocs Drive, it reinstalls **Message Queuing** for you\. For more help, contact your administrator\.

## Drive Repair Required<a name="ts-2"></a>

**Windows** – Restart by opening the Amazon WorkDocs Drive settings and choosing **Log out \(change site\)**\. Repeat those steps to sign in again, and then check the `Recovered Files` folder for any files you might need to save\. If you don't remember how to open the settings, see [Opening the Amazon WorkDocs Drive settings](open-wdd-settings.md)\.

**MacOS** – Restart Amazon WorkDocs Drive by choosing the **Amazon WorkDocs Drive** icon on the menu bar, choosing the gear icon, then choosing **Log out**\. Repeat those steps to sign in again, and then check the `Recovered Files` folder for any files you might need to save\.

## Kernel extensions version mismatch<a name="ts-3"></a>

If you use a Mac, you may see the following **Version Mismatch** notification when you try to launch WorkDocs Drive:

 ![\[Notice saying that macFUSE has been updated, but the system has an older version.\]](http://docs.aws.amazon.com/workdocs/latest/userguide/images/wd-version-mismatch-notice.jpg) 

This happens when a WorkDocs Drive update uses a new kernel extension\. Follow these steps to fix the issue\.

**To fix the mismatch**

1. Restart your machine\. This unloads the current extension\.

1. Try to start Amazon WorkDocs Drive\. Your OS blocks the new kernel extension and prompts you to allow it\.

1. Go to **System Preferences**, then **Security and Privacy**, and allow the extension\.

    ![\[Notice saying the system extension was updated.\]](http://docs.aws.amazon.com/workdocs/latest/userguide/images/wd-mismatch-update-ok.png) 

1. Restart your machine\. This loads the new kernel extension\.

1. Start Amazon WorkDocs Drive\.

## Local Disk Full<a name="ts-4"></a>

Delete unnecessary files from your local disk and `Recovered Files` folder\.

## Recovered Files<a name="ts-5"></a>

If you change a file that you don't have permissions to edit, you can't upload that file to your Amazon WorkDocs site\. Instead, the site saves the changes to your local `Recovered Files` folder\. You can open this folder from the Amazon WorkDocs Drive menu by choosing the question mark icon, then **Go to recovery folder**\. From there, you can upload the file to Amazon WorkDocs as a new file\.

## Recovery Folder Full<a name="ts-6"></a>

Delete unnecessary files from your local `Recovered Files` folder\.

## Storage Limit Exceeded<a name="ts-7"></a>

Delete unused files to free up storage space\. If you need more space after deleting unused files, contact your Amazon WorkDocs administrator\.

## Newer version already installed<a name="ts-8"></a>

Follow these steps:

**To fix the error**

1. Remove your current version of Amazon WorkDocs Drive For more information, see [Uninstalling Amazon WorkDocs Drive](uninstall.md)\.

1. Restart your machine\.

1. Install Amazon WorkDocs Drive\. For more information, see [Installing Amazon WorkDocs Drive](drive_install.md)\.