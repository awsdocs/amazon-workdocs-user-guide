# Using the Windows Subsystem for Linux to mount Amazon WorkDocs Drive<a name="mount-linux"></a>

If you run the Windows Subsystem for Linux, you can use the following `Bash` commands to mount Amazon WorkDocs Drive for PC \. For more information, see [File System Improvements to the Windows Subsystem for Linux](http://aws.amazon.com/blogs/wsl/2017/04/18/file-system-improvements-to-the-windows-subsystem-for-linux/)\.

```
$ sudo mkdir /mnt/w
$ sudo mount -t drvfs W: /mnt/w
$ cd /mnt/w
$ ls
```