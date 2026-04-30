---
title: "OPCSetMode"
description: "Specifies the communication mode for an OPC block."
---

# OPCSetMode

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetMode

Specifies the communication mode for an OPC block.

## Signature

```python
dd.OPCSetMode(OPCMode)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table17">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetMode(<em>ComMode</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCMode</td>
<td>Specifies the communication mode between an OPC block and an OPC server.<div id="exp_OPCMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCMode &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCMode</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>The communication is synchronous.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>The communication is asynchronous.</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetMode.htm`*
