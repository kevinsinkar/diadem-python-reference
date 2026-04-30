---
title: "PkWFactor"
description: "Specifies in packet processing to what extent DIAdem uses data of previous data packets to calculate the mean value. If you assign the value 1 to the PkWFactor "
---

# PkWFactor

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkWFactor

Specifies in packet processing to what extent DIAdem uses data of previous data packets to calculate the mean value. If you assign the value 1 to the PkWFactor variable, DIAdem weights all data in a data packet equally. The smaller the weighting factor you select, the less previously calculated data packets are used to calculate the mean value.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkWFactor</donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkwfactor.htm`*
