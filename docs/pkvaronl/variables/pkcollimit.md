---
title: "PkColLimit"
description: "Specifies in packet processing that the voltmeter highlights in color when the limit values are exceeded or undershot. The voltmeter displays the valid value ra"
---

# PkColLimit

!!! abstract "Variable &middot; `PkVarOnl.chm`"
    Variable: PkColLimit

Specifies in packet processing that the voltmeter highlights in color when the limit values are exceeded or undershot. The voltmeter displays the valid value range in green, the warning range in yellow, and the alarm range in red.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/>
 <donottranslate><pre>DACObjOpen(<em>BlockName</em>)
    <donottranslate>PkColLimit(i)</donottranslate> = <em>Value</em>
DACObjClose(<em>BlockName</em>)</pre>
</donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

---

*Source: `PkVarOnl/pkvaronl/pkcollimit.htm`*
