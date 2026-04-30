---
title: "PkSizeMax"
description: "Specifies for the section creation in packet processing the maximum number of values that DIAdem collects and outputs through a control signal, in a data packet"
---

# PkSizeMax

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkSizeMax

Specifies for the section creation in packet processing the maximum number of values that DIAdem collects and outputs through a control signal, in a data packet. DIAdem does not create data packets with a large packet size.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
     <donottranslate>PkSizeMax </donottranslate>= <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pksizemax.htm`*
