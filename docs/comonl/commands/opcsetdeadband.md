---
title: "OPCSetDeadBand"
description: "Specifies the deadband of an OPC block that works asynchronously."
---

# OPCSetDeadBand

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetDeadBand

Specifies the deadband of an OPC block that works asynchronously.

## Signature

```python
dd.OPCSetDeadBand(OPCDeadBand)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table10">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetDeadBand(<em>Value</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCDeadBand</td>
<td>Specifies the deadband as a percentage.<div id="exp_OPCDeadBand">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= OPCDeadBand &lt;= 100</td></tr>
</table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetDeadBand.htm`*
