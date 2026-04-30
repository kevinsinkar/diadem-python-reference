---
title: "PkAlAppend"
description: "Specifies whether DIAdem deletes and recreates the logfile at the beginning of a measurement. If you assign the value FALSE to the PkAlAppend variable, DIAdem c"
---

# PkAlAppend

!!! abstract "Variable &middot; `Gfsalarm.chm`"
    Variable: PkAlAppend

Specifies whether DIAdem deletes and recreates the logfile at the beginning of a measurement. If you assign the value FALSE to the PkAlAppend variable, DIAdem creates a new logfile. If you assign the value TRUE to the PkAlAppend variable, DIAdem appends new logfile entries to the existing entries.

## Notes

<div markdown="1">
<table class="Borderless" id="table4"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    PkAlAppend = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

---

*Source: `Gfsalarm/pkalappend.htm`*
