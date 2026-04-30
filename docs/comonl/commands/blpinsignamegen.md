---
title: "BlPinSigNameGen"
description: "Overwrites in terminals of blocks and subblock diagrams the terminal names with the signal names."
---

# BlPinSigNameGen

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: BlPinSigNameGen

Overwrites in terminals of blocks and subblock diagrams the terminal names with the signal names.

## Signature

```python
dd.BlPinSigNameGen(BlName, SchemeLev, BlPinNo)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlPinNo = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">BlName</td>
<td>Specifies the name of a DAC block.<div id="exp_BlName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 16 characters</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SchemeLev</td>
<td>Specifies the bus layer.<div id="exp_SchemeLev">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
<td>0 &lt;= SchemeLev &lt;= 6</td></tr>
</table>
<p class="Body">The <span class="Monospace">SchemeLev</span> variable can contain the following values:</p>
<table class="Borderless" id="table2">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr>
<td width="150"><pre><donottranslate>0</donottranslate></pre>
</td>
<td>The signal buses are on the data layer.</td>
</tr>
<tr>
<td width="150"><pre><donottranslate>1</donottranslate></pre></td>
<td>The signal buses are on the control layer.</td>
</tr>
<tr>
<td width="150"><pre><donottranslate>2</donottranslate></pre></td>
<td>The signal buses are on the system layer.</td>
</tr>
<tr>
<td width="150"><pre><donottranslate>3</donottranslate></pre></td>
<td>The signal buses are on the packet layer.</td>
</tr>
<tr>
<td width="150"><pre><donottranslate>4</donottranslate></pre></td>
<td>The signal buses are on the alarm layer.</td>
</tr>
<tr>
<td width="150"><pre><donottranslate>5</donottranslate></pre></td>
<td>The signal buses are on the text layer.</td>
</tr>
</table>
<p>
</p></div></td></tr>
<tr><td width="150">BlPinNo</td>
<td>Specifies the number of the block terminal.<div id="exp_BlPinNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlPinNo = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/BlPinSigNameGen.htm`*
