---
title: "OPCSetItemID"
description: "Sets the OPC item for a signal and generates the signal name."
---

# OPCSetItemID

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetItemID

Sets the OPC item for a signal and generates the signal name.

## Signature

```python
dd.OPCSetItemID(OPCSigIndex, OPCItemID)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table14"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the OPC signal has the status <span class="Monospace">Undefined</span>, the <span class="Monospace">OPCSetItemID</span> command creates the signal name from the ItemID and sets the status to <span class="Monospace">Defined</span>. If the OPC signal already has the status <span class="Monospace">Defined</span>, this command changes the ItemID without changing the signal name.</td></tr></table>
<table class="Borderless" id="table15">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetItemID(<em>SignalIndex,ItemID</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
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
<tr><td width="150">OPCItemID</td>
<td>Specifies the identifier of an OPC item.<div id="exp_OPCItemID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 80 characters</td></tr>
</table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150">OPCSigName</td>
<td>Receives the name of a signal in an OPC block.<div id="exp_OPCSigName">
<table class="Borderless">
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

*Source: `ComOnl/OPCSetItemID.htm`*
