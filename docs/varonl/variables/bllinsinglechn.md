---
title: "BlLinSingleChn"
description: "Specifies whether each signal uses its own interpolation channel pair, or whether all signals use one mutual interpolation channel pair. If the value is TRUE , "
---

# BlLinSingleChn

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlLinSingleChn

Specifies whether each signal uses its own interpolation channel pair, or whether all signals use one mutual interpolation channel pair. If the value is TRUE , DIAdem uses a separate interpolation channel pair for each signal.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlLinSingleChn = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

---

*Source: `VarOnl/BlLinSingleChn.htm`*
