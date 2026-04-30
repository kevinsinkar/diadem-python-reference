---
title: "PkAlConfirmAll"
description: "Specifies whether DIAdem confirms all the alarms that are selected in the table. If you assign the value 1 to the PkAlConfirmAll variable, DIAdem confirms all t"
---

# PkAlConfirmAll

!!! abstract "Variable &middot; `Gfsalarm.chm`"
    Variable: PkAlConfirmAll

Specifies whether DIAdem confirms all the alarms that are selected in the table. If you assign the value 1 to the PkAlConfirmAll variable, DIAdem confirms all the alarms. Otherwise, DIAdem confirms only the selected alarms.

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    PkAlConfirmAll = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

---

*Source: `Gfsalarm/pkalconfirmall.htm`*
