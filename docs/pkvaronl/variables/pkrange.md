---
title: "PkRange"
description: "Specifies in packet processing the width of all classes of an online classification."
---

# PkRange

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkRange

Specifies in packet processing the width of all classes of an online classification.

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Do not change the value of the variable after you have started a measurement. If you want to change a variable during a measurement, you must first reset the internal buffer.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkRange</donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkkrange.htm`*
