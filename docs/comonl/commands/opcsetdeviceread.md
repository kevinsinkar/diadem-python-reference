---
title: "OPCSetDeviceRead"
description: "Specifies how an OPC block reads in data."
---

# OPCSetDeviceRead

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetDeviceRead

Specifies how an OPC block reads in data.

## Signature

```python
dd.OPCSetDeviceRead(OPCDeviceRead)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table13">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetDeviceRead(<em>Value</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCDeviceRead</td>
<td>Specifies the type of read access for an OPC block.<div id="exp_OPCDeviceRead">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCDeviceRead &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCDeviceRead</span> variable can contain the following values:</p>
<table class="Borderless" id="table1">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>The OPC block contains the values in a buffer.</td>
</tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>The OPC block reads the values directly from the OPC signals.</td>
</tr></table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetDeviceRead.htm`*
