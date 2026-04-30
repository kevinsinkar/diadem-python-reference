---
title: "PkMode"
description: "Specifies in packet processing how DIAdem extracts data from incoming data packets."
---

# PkMode

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkMode

Specifies in packet processing how DIAdem extracts data from incoming data packets.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note </strong> Do not assign values <span class="Monospace">3</span> or <span class="Monospace">4</span> to the <span class="Monospace">PkMode</span> variable if you have started a measurement. These settings block the packet processing, because DIAdem cannot create a control input during a measurement.</td>
</tr>
</table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>

 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkMode</donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkrmode.htm`*
