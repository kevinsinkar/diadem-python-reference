---
title: "BlExtAppName"
description: "Specifies an external application to be launched or the title of a window to be displayed."
---

# BlExtAppName

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlExtAppName

Specifies an external application to be launched or the title of a window to be displayed.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlExtAppName = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To execute the application you must specify the program name, the path, and the parameters of the program you want to launch.</td></tr></table>
</div>

---

*Source: `VarOnl/BlExtAppName.htm`*
