# Transferring folder ownership<a name="transfer-owner"></a>

You can request a transfer of ownership for any folders that you own\. Remember the following:
+ Transferring a folder automatically transfers ownership of all the files in that folder\.
+ Transfers remove ownership from you and grant it to a user that you specify\.
+ The specified user must accept ownership\. You retain ownership until the other user accepts\.

**Note**  
System administrators can transfer an inactive user's files and folders to an active user\. For more information, see [Transferring document ownership](https://docs.aws.amazon.com/workdocs/latest/adminguide/transfer-docs.html) in the *Amazon WorkDocs Administration Guide*\.

**To transfer ownership folders**

1. Use the credentials provided by your administrator to log in to the Amazon WorkDocs web client\.

1. On your **My Docs** page, select the check box next to the folder that you want to transfer\.
**Note**  
Don't select the folder name\. Doing so opens the folder in Preview mode and disables the **Transfer** command\. Just select the check boxes\.

1. Open the **Actions** list and choose **Transfer**\.

   The **Transfer Resource Ownership** dialog box appears\.

1. In the search box, enter the name of the new owner\. If the search returns multiple names, choose the correct recipient\.

1. Choose **Transfer**\.

The new owner receives a task under **My Tasks** in Amazon WorkDocs\. After the new owner accepts the files, they appear on that owner's **My Docs** page\.