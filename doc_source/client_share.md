# Sharing a Folder or File<a name="client_share"></a>

You can share a folder or file with other users and groups both within and outside your organization\. You can also revoke the share, and the users can remove themselves from the share\.

**Limits**

+ You can only share with directory groups, not email distribution lists\.

+ If your administrator configured Amazon WorkDocs with AD Connector, you can't share with users outside the directory\.


+ [Share a Folder or File](#share)
+ [Revoke a Share](#revoke_share)
+ [Remove Yourself from a Share](#unshare_yourself)

## Share a Folder or File<a name="share"></a>

You can share a folder or file with other users and groups both within and outside your organization using **Share by invite**\. In addition, you can specify the type of access permissions when inviting a user\.

**To share a folder or file with other users and groups**

1. In the web client, open the folder or file\.

1. In the control pane, choose **Share by invite**\. 

1. In the **Share by invite** dialog box, start typing the name of the person or group in your organization with whom to share, and select the desired name when it is displayed in the list\. If your Amazon WorkDocs administrator has authorized you to share files with people outside your organization, you can also enter email addresses for external people and add them to the list of people with whom to share the folder or file\. 

   Repeat this step for any others you want to share the file with\.

1. Select the desired permissions for the folder or file\.  
**Co\-Owner**  
The users/groups are co\-owners of the file or files in the folder\. They can rename and delete files, and share the file or files with others\.  
**Contributor**  
The users/groups can provide feedback on the file or files in the folder\.  
**Viewer**  
The users/groups can only view the file or files in the folder\. They cannot provide feedback\. External users have **Viewer** as the default permission, and this can't be changed unless they are converted from a **Guest** to regular **User** by an administrator\.

1. Enter a personal message \(if desired\) of no more than 2048 characters, and select if feedback is requested\. If feedback is requested, you can optionally specify a deadline for receiving feedback\.
**Note**  
Feedback can only be requested for files, not folders\. Feedback can only be requested from users, not groups\.

1. Choose **OK**\. 

An email is sent to the people notifying them that a file has been shared with them\. The email includes a web link to the file, the personal message that was entered, and the feedback deadline, if one was specified\. The users/groups, along with their assigned role, are also added to the People tab\. If you receive an error message that indicates that you cannot share a document with people outside of your organization, your administrator has not authorized you to invite new users to the organization\. Contact your Amazon WorkDocs administrator for assistance\.

## Revoke a Share<a name="revoke_share"></a>

After you have shared a folder or file, you can remove a user or groups from the share\.

**To revoke a share**

1. In the web client, open the folder or file\.

1. In the control pane, choose **People**\.

1. From the list of people that the folder or file is shared with, choose **Close** next to the user or group to remove from the share list\.

1. In the confirmation dialog box, choose **Remove It**\. The user or group is immediately removed from the share list\.

## Remove Yourself from a Share<a name="unshare_yourself"></a>

After a folder or file has been shared with you, you can remove yourself from the share if desired\.

**To remove yourself from a share**

1. In the web client, open the folder that contains the folder or file that has been shared with you\.

1. Choose the arrow for the item and **Remove me from share**\.

1. In the confirmation dialog box, choose **Yes, remove me**\. You immediately lose access to the share\.