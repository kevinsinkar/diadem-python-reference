---
title: "BlStartInterv"
description: "Specifies the number of values that DIAdem saves before the start trigger, or that DIAdem rejects after the start trigger."
---

# BlStartInterv

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlStartInterv

Specifies the number of values that DIAdem saves before the start trigger, or that DIAdem rejects after the start trigger.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlStartInterv(i) = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The pre-trigger range must be smaller than the number of values to be saved.</td></tr></table>
</div>

---

*Source: `VarOnl/BlStartInterv.htm`*
