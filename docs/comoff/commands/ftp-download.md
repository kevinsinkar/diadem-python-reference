---
title: "FTP download"
description: "Downloads a file from an FTP server."
---

# FTP download

!!! abstract "Command &middot; `ComOff.chm`"
    Command: FTP download

Downloads a file from an FTP server.

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
<tr><td width="150">FTPSourcePath</td>
<td>Specifies the source path. The parameter <span class="Monospace">FTPSourcePath</span> is case sensitive.<div id="exp_FTPSourcePath">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">FTPFileName</td>
<td>Specifies the filename. The file name may also contain wildcards. The parameter FTPFileName is case sensitive.<div id="exp_FTPFileName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">FTPTargetPath</td>
<td>Specifies the target path.<div id="exp_FTPTargetPath">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[FTPTimeout]</td>
<td>Specifies in seconds the time that elapses before DIAdem times out the connection attempt.<div id="exp_FTPTimeout">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>1 &lt;= FTPTimeout &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[FTPRetry]</td>
<td>Specifies whether DIAdem retries sending lost data packets following a timeout.<div id="exp_FTPRetry">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= FTPRetry &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives information as to whether the FTP connection was successful. The return value is a FTPState type.<div id="exp_FTPState">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"FTPNoError"</pre></donottranslate></td>
<td>No error.</td></tr>
<tr><td width="150"><donottranslate><pre>"FTPError"</pre></donottranslate></td>
<td>Error</td></tr>
<tr><td width="150"><donottranslate><pre>"FTPTimeout"</pre></donottranslate></td>
<td>Timeout</td></tr>
<tr><td width="150"><donottranslate><pre>"FTPAbort"</pre></donottranslate></td>
<td>Abort</td></tr>
</table>
</td></tr>
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

*Source: `ComOff/FTPDownload.htm`*
