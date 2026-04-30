---
title: "PkHoldPack"
description: "Specifies in packet processing whether DIAdem saves data packets at inactive data inputs of the multiplexer to the clipboard and does not reject the data packet"
---

# PkHoldPack

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkHoldPack

Specifies in packet processing whether DIAdem saves data packets at inactive data inputs of the multiplexer to the clipboard and does not reject the data packets. DIAdem always evaluates data packets at the control input.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkHoldPack</donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkholdpack.htm`*
