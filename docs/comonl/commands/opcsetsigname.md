---
title: "OPCSetSigName"
description: "Specifies a new unique name for an OPC signal."
---

# OPCSetSigName

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetSigName

Specifies a new unique name for an OPC signal.

## Signature

```python
dd.OPCSetSigName(OPCSigIndex, OPCSigName)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table18">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetSigName(<em>SignalIndex,SignalName</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCSigIndex</td>
<td>Specifies the index of a signal in an OPC block.<div id="exp_OPCSigIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCSigIndex &lt;= 2147483647</td></tr>
</table>
<p>The index starts with <span class="Monospace">1</span>.</p>
</div></td></tr>
<tr><td width="150">OPCSigName</td>
<td>Specifies the name of a signal in an OPC block.<div id="exp_OPCSigName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 80 characters</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless" id="table16">
<tr>
<td width="150"> OPCSigName</td>
<td>Receives the name of a signal in an OPC block.<div id="exp_OPCSigName_1">
<table class="Borderless" id="table17">
<tr>
<td><a href="#" data-unresolved="1">String variable</a></td>
</tr>
<tr>
<td>Maximum 80 characters</td>
</tr>
</table>
</div>
</td>
</tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetSigName.htm`*
