# Understanding when Amazon WorkDocs creates versions<a name="version-creation"></a>

As a rule, Amazon WorkDocs creates file versions when you overwrite a file or save changes to a file\. However, that process varies, depending on where you are and what you do with a file\.

**From the Amazon WorkDocs web client**  
When you upload a file to the web client, and that file already exists in the same folder, the uploaded file becomes the new version\.  
Also, when you preview a file in the web client, and you then drag any file from your local drive and drop it onto the previewed file, the dropped file becomes the new version\.

**From Amazon WorkDocs Companion**  
If you edit a file while using Companion, Amazon WorkDocs creates a new version each time you save the file\.

**From Amazon WorkDocs Drive**  
When you edit a file stored in Amazon WorkDocs Drive the system creates a new version every 30 seconds while you edit\.  
Amazon WorkDocs Drive can create versions of large files that consume a lot of your storage space\. For information on how to reduce the amount of storage, see the next section\.