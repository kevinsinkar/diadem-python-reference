---
title: "PkPeriod"
description: "Specifies in hours, minutes, and seconds how long the timer of the packet processing outputs a control signal. At the end of the run-time the control signal fal"
---

# PkPeriod

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkPeriod

Specifies in hours, minutes, and seconds how long the timer of the packet processing outputs a control signal. At the end of the run-time the control signal falls to TTL low.

## Notes

<div markdown="1">
<table class="Borderless" id="table2">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Do not change the value of a measurement after the measurement has started.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkPeriod </donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkperiod.htm`*
