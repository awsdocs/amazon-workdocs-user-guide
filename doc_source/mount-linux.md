# Using the Windows Subsystem for Linux to mount Amazon WorkDocs Drive<a name="mount-linux"></a>

If you run the Windows Subsystem for Linux, you can use the following `Bash` commands to mount Amazon WorkDocs Drive for PC\.

```
$ sudo mkdir /mnt/w
$ sudo mount -t drvfs W: /mnt/w
$ cd /mnt/w
$ ls
```