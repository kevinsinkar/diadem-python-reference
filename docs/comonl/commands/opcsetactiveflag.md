---
title: "OPCSetActiveFlag"
description: "Enables or disables the signals in an OPC block."
---

# OPCSetActiveFlag

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetActiveFlag

Enables or disables the signals in an OPC block.

## Signature

```python
dd.OPCSetActiveFlag(OPCSigIndex, OPCActiveFlag)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table4">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/>
<br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetActiveFlag(<em>SignalIndex,1</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
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
<tr><td width="150">OPCActiveFlag</td>
<td>Specifies whether a signal of an OPC block is active.<div id="exp_OPCActiveFlag">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCActiveFlag &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCActiveFlag</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>The OPC signal is not active.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>The OPC signal is active.</td></tr></table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetActiveFlag.htm`*
