---
title: "PkAutoScalOn"
description: "Specifies in packet processing that DIAdem scales the y-axis of the oscilloscope like the incoming data packets. If you assign the value 0 to the PkAutoScalOn v"
---

# PkAutoScalOn

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkAutoScalOn

Specifies in packet processing that DIAdem scales the y-axis of the oscilloscope like the incoming data packets. If you assign the value 0 to the PkAutoScalOn variable, DIAdem scales the y-axis according to the specified start value and end value.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkAutoScalOn</donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate>
<br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkautoscalon.htm`*
