---
title: "BlLinChnX"
description: "Specifies the name of the channel that contains the measured values of a linearization function."
---

# BlLinChnX

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlLinChnX

Specifies the name of the channel that contains the measured values of a linearization function.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlLinChnX = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>For more information, refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a>.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The two channels with the x-values and the y-values of the linearization function must be in the Data Portal. For the linearization of inputs the x-channel must contain monotonous ascending values.</td></tr></table>
</div>

---

*Source: `VarOnl/BlLinChnX.htm`*
