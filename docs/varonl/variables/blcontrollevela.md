---
title: "BlControlLevelA"
description: "Specifies the lower limit for a 2-point controller and the lower switching point for a 3-point controller."
---

# BlControlLevelA

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlControlLevelA

Specifies the lower limit for a 2-point controller and the lower switching point for a 3-point controller.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlControlLevelA = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If the control difference undershoots the lower switch-on level specified by the <span class="Monospace">BlControlLevelA</span> variable in the 3-point controller, DIAdem sets the set point to the value <span class="Monospace">1</span>.</td></tr></table>
</div>

---

*Source: `VarOnl/BlControlLevelA.htm`*
