---
title: "FTPDisConnect"
description: "Disconnects from the FTP server."
---

# FTPDisConnect

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FTPDisConnect

Disconnects from the FTP server.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FTPConnectionHandle</td>
<td>Specifies the handle for the FTP connection.<div id="exp_FTPConnectionHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean variable</a> type. Receives the information whether DIAdem has successfully executed the command.</td></tr>
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

*Source: `ComOff/FTPDisConnect.htm`*
