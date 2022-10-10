# Naming files<a name="client-name-files"></a>

Before you create files in Amazon WorkDocs you need to know how to name them\. Incorrect characters in file names can cause your Amazon WorkDocs administrator several problems\. For example, your administrator can't migrate your data to a faster server or a different user group\. Here's a list of what to look for and avoid\.
+ **Trailing spaces** – For example: an extra space at the end of a file name\.
+ **Periods at the beginning or end** – For example: `.file`, `.file.ppt`, `.`, `..`, or `file.`
+ **Tildes at the beginning or end** – For example: `file.doc~`, `~file.doc`, or `~$file.doc`
+ **File names ending in `.tmp`** – For example: `file.tmp`
+ **File names exactly matching these case\-sensitive terms** – `Microsoft User Data`, `Outlook files`, `Thumbs.db`, or `Thumbnails`
+ **File names containing any of these characters** – `*` \(asterisk\), `/` \(forward slash\), `\` \(back slash\), `:` \(colon\), `<` \(less than\), `>` \(greater than\), `?` \(question mark\), `|` \(vertical bar/pipe\), `"` \(double quotes\), or `\202E` \(character code 202E\)\.