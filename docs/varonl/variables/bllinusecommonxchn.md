---
title: "BlLinUseCommonXChn"
description: "Specifies whether DIAdem uses a common input channel in the free linearization through channels. If the value is TRUE , DIAdem uses one common input channel. Yo"
---

# BlLinUseCommonXChn

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlLinUseCommonXChn

Specifies whether DIAdem uses a common input channel in the free linearization through channels. If the value is TRUE , DIAdem uses one common input channel. You must assign the value TRUE to the BlLinSingleChn variable so that DIAdem includes the BlLinUseCommonXChn variable.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlLinUseCommonXChn = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>For more information, refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a>.</td></tr></table>
</div>

---

*Source: `VarOnl/BlLinUseCommonXChn.htm`*
