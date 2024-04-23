# LabVIEW-Program-run-on-startup
LabVIEW范例：如何让程序在系统启动时自启动


## 需要了解

1. [MSDN:Run and RunOnce Registry Keys](https://learn.microsoft.com/en-us/windows/win32/setupapi/run-and-runonce-registry-keys?redirectedfrom=MSDN)

```text
Use Run or RunOnce registry keys to make a program run when a user logs on.
The Run key makes the program run every time the user logs on,
while the RunOnce key makes the program run one time, and then the key is deleted.
These keys can be set for the user or the machine.

The data value for a key is a command line no longer than 260 characters.
Register programs to run by adding entries of the form description-string=commandline.
You can write multiple entries under a key.
If more than one program is registered under any particular key,
the order in which those programs run is indeterminate.

The Windows registry includes the following four Run and RunOnce keys:

HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run
HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\RunOnce
HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run
HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\RunOnce

```

1. [Pass Command Line Arguments to a LabVIEW Executable](https://knowledge.ni.com/KnowledgeArticleDetails?id=kA03q000000YHdICAW&l=en-US)

![image](.doc/Snipaste_2024-04-23_10-38-19.png)