# Uninstalling Amazon WorkDocs Drive<a name="uninstall"></a>

These steps explain how to uninstall Amazon WorkDocs Drive from Windows MacOS, and Apple silicon machines\. 

**To uninstall Amazon WorkDocs Drive from Windows machines**

1. Open the Amazon WorkDocs Drive settings and choose **Quit Amazon WorkDocs Drive**\. If you don't remember how to open the settings, see [Opening the Amazon WorkDocs Drive settings](open-wdd-settings.md)\.

1. Start **Control Panel**, choose **Programs and Features**, **Amazon WorkDocs Drive**, **Uninstall**, and then choose **OK**\.

**To uninstall Amazon WorkDocs Drive from MacOS Intel machines**

1. On the menu bar, choose the Amazon WorkDocs Drive icon, choose the gear icon, then choose **Quit Amazon Workdocs Drive**\.

1. From the **Applications** folder, choose the Amazon WorkDocs Drive icon, then choose **Move to Trash**\. 

1. Navigate to **\~/\.config/Amazon/AWSWorkDocsDriveClient** on your hard dive and remove the **WorkDocs** folder and any sub folders\. Finally, navigate to **\~/Library/Caches/** and empty your WorkDocs cache\.

You can remove Amazon WorkDocs Drive from MacOS Apple silicon machines manually by using the **Applications** folder, or you can use the command line\. The following steps explain how to use both methods\.

**To uninstall Amazon WorkDocs Drive from MacOS Apple silicon devices \(manual\)**

1. Open the **Applications** folder\.

1. Open the **WorkDocs Drive** context menu and choose **Show package contents**\.

1. Select the **MacOS** folder\.

1. Tap and hold \(double\-click\) to uninstall Amazon WorkDocs Drive\.

**To uninstall Amazon WorkDocs Drive from MacOS Apple silicon devices \(command line\)**
+ Open Terminal and run the following command\. Enter the command on a single line no line breaks, and enter your password when prompted to enter your password

  `sudo /Applications/WorkDocs\[Drive\.app/Contents/MacOS/uninstall\.app/Contents/MacOs/uninstall](http://drive.app/Contents/MacOS/uninstall.app/Contents/MacOs/uninstall).`