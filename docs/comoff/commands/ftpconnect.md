---
title: "FTPConnect"
description: "Connects to an FTP server."
---

# FTPConnect

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FTPConnect

Connects to an FTP server.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FTPServerName</td>
<td>Specifies the name or the IP address of the server or the FTP connection.<div id="exp_FTPServerName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[FTPUserName]</td>
<td>Specifies the user name for the FTP connection.<div id="exp_FTPUserName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[FTPPassword]</td>
<td>Specifies the password for the FTP connection.<div id="exp_FTPPassword">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Specifies the handle for the FTP connection. The return value is a FTPConnectionHandle type.<div id="exp_FTPConnectionHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
iFTPHandle = dd.FTPConnect("ftp.ni.com") #Server name, you can also use the IP adress

if iFTPHandle > 0 :
    FTPDownloadState = dd.FTPDownload(iFTPHandle,"/.","README.txt", "d:\\")

    select_variable_0 = FTPDownloadState
    if (select_variable_0 == "FTPNoError") :
        print("No error")
    elif (select_variable_0 == "FTPError") :
        print("An error occured")
    elif (select_variable_0 == "FTPTimeout") :
        print ("Timeout")
    elif (select_variable_0 == "FTPAbort") :
        print ("Cancel")

    dd.FTPDisconnect(iFTPHandle)
else:
    print("Could not connect to the server.")
```

```python
iFTPHandle = dd.FTPConnect("130.164.81.30") #Server name, you can also use the IP adress

if iFTPHandle > 0 :
    FTPDownloadState = dd.FTPDownload(iFTPHandle,"/.","README.txt", "d:\\")

    select_variable_0 = FTPDownloadState
    if (select_variable_0 == "FTPNoError") :
        print("No error")
    elif (select_variable_0 == "FTPError") :
        print("An error occured")
    elif (select_variable_0 == "FTPTimeout") :
        print ("Timeout")
    elif (select_variable_0 == "FTPAbort") :
        print ("Cancel")

    dd.FTPDisconnect(iFTPHandle)
else:
    print("Could not connect to the server.")
```

---

*Source: `ComOff/FTPConnect.htm`*
