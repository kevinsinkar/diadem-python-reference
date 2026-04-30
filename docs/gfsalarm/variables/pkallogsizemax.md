---
title: "PkAlLogSizeMax"
description: "Specifies the size that the logfile has to reach for DIAdem to reset the logfile. If you assign the value 0 to the PkAlLogSizeMax variable, DIAdem does not rese"
---

# PkAlLogSizeMax

!!! abstract "Variable &middot; `Gfsalarm.chm`"
    Variable: PkAlLogSizeMax

Specifies the size that the logfile has to reach for DIAdem to reset the logfile. If you assign the value 0 to the PkAlLogSizeMax variable, DIAdem does not reset the logfile.

## Notes

<div markdown="1">
<table class="Borderless" id="table16"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    PkAlLogSizeMax = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

---

*Source: `Gfsalarm/pkallogsizemax.htm`*
