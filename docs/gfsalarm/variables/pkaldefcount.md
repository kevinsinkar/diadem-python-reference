---
title: "PkAlDefCount"
description: "Specifies the number of alarm definitions in the alarm generator. If you enter a number that is lower than the number that the alarm generator contains, DIAdem "
---

# PkAlDefCount

!!! abstract "Variable &middot; `Gfsalarm.chm`"
    Variable: PkAlDefCount

Specifies the number of alarm definitions in the alarm generator. If you enter a number that is lower than the number that the alarm generator contains, DIAdem rejects the remaining alarm definitions.

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    PkAlDefCount = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

---

*Source: `Gfsalarm/pkaldefcount.htm`*
