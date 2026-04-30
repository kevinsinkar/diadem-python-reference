---
title: "BlControlUseLastOutputOnNoInput"
description: "Specifies that DIAdem outputs the previous value when a NoValue value arrives at the controller as a set point or as an actual value. This prevents the controll"
---

# BlControlUseLastOutputOnNoInput

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlControlUseLastOutputOnNoInput

Specifies that DIAdem outputs the previous value when a NoValue value arrives at the controller as a set point or as an actual value. This prevents the controller from outputting only NoValues after a single NoValue value. However, DIAdem cannot control while DIAdem processes the NoValue value. Therefore, the time in which the controller receives NoValue values should be as short as possible.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlControlUseLastOutputOnNoInput = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

---

*Source: `VarOnl/BlControlUseLastOutputOnNoInput.htm`*
