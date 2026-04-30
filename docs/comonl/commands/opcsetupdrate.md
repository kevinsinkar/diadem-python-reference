---
title: "OPCSetUpdRate"
description: "Specifies the time after which the OPC server regularly updates the data in the OPC group."
---

# OPCSetUpdRate

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetUpdRate

Specifies the time after which the OPC server regularly updates the data in the OPC group.

## Signature

```python
dd.OPCSetUpdRate(OPCUpdRate)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table17">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetUpdRate(<em>Rate</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCUpdRate</td>
<td>Specifies the rate in milliseconds at which the OPC server regularly updates the data in the OPC group.<div id="exp_OPCUpdRate">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCUpdRate &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetUpdRate.htm`*
