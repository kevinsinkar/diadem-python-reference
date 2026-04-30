---
title: "OPCSetArrAccess"
description: "Enables array indexing for the signals of an OPC block."
---

# OPCSetArrAccess

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetArrAccess

Enables array indexing for the signals of an OPC block.

## Signature

```python
dd.OPCSetArrAccess(OPCSigIndex, OPCArrayEnable, OPCArrayIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table5">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/>
<br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetArrAccess(<em>SignalIndex</em>,<em>1</em>,<em>ArrayIndex</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
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
<tr><td width="150">OPCArrayEnable</td>
<td>Specifies whether array indexing is executed for a signal in an OPC block.<div id="exp_OPCArrayEnable">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCArrayEnable &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCArrayEnable</span> variable can contain the following values:</p><table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>No array indexing for signal.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>Array indexing for signal.</td></tr></table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">OPCArrayIndex</td>
<td>Specifies the index of the read value when the OPC server returns an array for the OPC item.<div id="exp_OPCArrayIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCArrayIndex &lt;= 2147483647</td></tr>
</table>
<p>The array length limits the value range.</p>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetArrAccess.htm`*
