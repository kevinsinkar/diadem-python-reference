---
title: "OPCSyncListLen"
description: "Adjusts the length of the signal list of an OPC block to the current signal list of the DAC block diagram."
---

# OPCSyncListLen

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSyncListLen

Adjusts the length of the signal list of an OPC block to the current signal list of the DAC block diagram.

## Signature

```python
dd.OPCSyncListLen()
```

## Notes

<div markdown="1">
<table class="Borderless" id="table18">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSyncListLen()<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSyncListLen.htm`*
