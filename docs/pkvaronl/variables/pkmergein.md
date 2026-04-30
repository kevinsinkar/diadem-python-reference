---
title: "PkMergeIn"
description: "Specifies in packet processing the number of signal inputs from which DIAdem collects data packets and merges the data packets to a new multi-channel data packe"
---

# PkMergeIn

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkMergeIn

Specifies in packet processing the number of signal inputs from which DIAdem collects data packets and merges the data packets to a new multi-channel data packet.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Do not change the value of a measurement after the measurement starts.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkMergeIn</donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkmergein.htm`*
