---
title: "BlActPinSigOutp"
description: "Specifies the name of a signal at the open block output."
---

# BlActPinSigOutp

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlActPinSigOutp

Specifies the name of a signal at the open block output.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
  Call DACObjOpen(<em>ConnectorName</em>)
    BlActPinSigOutp(i) = <em>Value</em>
  Call DACObjClose(<em>ConnectorName</em>)
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block. You need the terminal name to open the signal terminal, to access the variable, and to close the signal terminal and the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

---

*Source: `VarOnl/BlActPinSigOutp.htm`*
