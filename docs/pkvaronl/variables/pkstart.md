---
title: "PkStart"
description: "Specifies in hours, minutes, and seconds when the timer sets the control signal in packet processing to TTL high . Use the syntax hh:mm:ss ."
---

# PkStart

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkStart

Specifies in hours, minutes, and seconds when the timer sets the control signal in packet processing to TTL high . Use the syntax hh:mm:ss .

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Do not change the value of a measurement after the measurement has started.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen</pre></donottranslate>(<em>BlockName</em>) <donottranslate>PkStart</donottranslate> = <em>Value</em> DACObjClose(<em>BlockName</em>)
     <br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkstart.htm`*
