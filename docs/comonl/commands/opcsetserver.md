---
title: "OPCSetServer"
description: "Specifies the OPC server with which an OPC block communicates."
---

# OPCSetServer

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetServer

Specifies the OPC server with which an OPC block communicates.

## Signature

```python
dd.OPCSetServer(OPCSrvName, OPCKeepList)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table19">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetServer(<em>ServerName,OPCList</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCSrvName</td>
<td>Specifies the name of an OPC server.<div id="exp_OPCSrvName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 80 characters</td></tr>
</table>
<p class="Body">You can specify server names as follows:</p>
<p class="Code1">&lt;ClassID&gt;</p>
<p class="Code1">&lt;ProgID&gt;</p>
<p class="Code1">&lt;Computername&gt;\&lt;ClassID&gt;</p>
<p class="Code1">&lt;Computername&gt;\&lt;ProgID&gt;</p>
<p class="Body">The ClassID identifies, globally unique, the COM object that is to be started, such as the OPC server. MS Windows always uses the ClassID when it starts OPC servers. The ProgID is the name of the OPC server, in text. MS Windows determines the associated ClassID from the registration of the OPC server with the operating system. The installation program writes the ClassID of the OPC server into the registration. However, if the OPC server is installed on a different computer, the registration of the local computer does not contain a ClassID for this OPC server. In this case you use the computer name and the ProgID.</p><p>
</p></div></td></tr>
<tr><td width="150">OPCKeepList</td>
<td>Specifies whether an OPC block maintains the existing signal list when the OPC server changes.<div id="exp_OPCKeepList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCKeepList &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCKeepList</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>The OPC block uses a new signal list.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>The OPC block keeps the current signal list.</td></tr></table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

## Python example

```python
dd.DACObjOpen("OPCInput")
OPCSetServer("MyComputer\\{B52C4D77-A715-11D2-9BC4-006008CA11C3}",1)
dd.DACObjClose("OPCInput")
```

```python
dd.DACObjOpen("OPCInput")
OPCSetServer("National Instruments.OPCDemo.1",1)
dd.DACObjClose("OPCInput")
```

---

*Source: `ComOnl/OPCSetServer.htm`*
