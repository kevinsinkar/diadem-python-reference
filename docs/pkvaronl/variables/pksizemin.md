---
title: "PkSizeMin"
description: "Specifies when sections are created in packet processing the minimum number of values that DIAdem needs to create a data packet when a control signal manages th"
---

# PkSizeMin

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkSizeMin

Specifies when sections are created in packet processing the minimum number of values that DIAdem needs to create a data packet when a control signal manages the control. DIAdem does not create data packets with smaller packet sizes.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkSizeMin </donottranslate>= <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pksizemin.htm`*
