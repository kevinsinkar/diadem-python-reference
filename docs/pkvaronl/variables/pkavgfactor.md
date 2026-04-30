---
title: "PkAvgFactor"
description: "Specifies in packet processing to what extent DIAdem uses previous data when calculating the current mean value for the FFT of two time signals. If you assign t"
---

# PkAvgFactor

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkAvgFactor

Specifies in packet processing to what extent DIAdem uses previous data when calculating the current mean value for the FFT of two time signals. If you assign the value 1 to the PkAvgFactor variable, DIAdem weights all data in a data packet equally. The smaller the weighting factor you select, the less previously calculated data packets are used to calculate the mean value.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkAvgFactor</donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate>
<br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkavgfactor.htm`*
