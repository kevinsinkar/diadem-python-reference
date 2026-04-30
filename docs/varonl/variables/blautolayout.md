---
title: "BlAutoLayout"
description: "Specifies whether DIAdem calculates the number of lines and the number of columns of the color matrix, or whether the user specifies the values."
---

# BlAutoLayout

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlAutoLayout

Specifies whether DIAdem calculates the number of lines and the number of columns of the color matrix, or whether the user specifies the values.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlAutoLayout = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If DIAdem specifies the number of lines and columns automatically, the matrix is always square. Therefore DIAdem might not display all connected signals with the color matrix.</td></tr></table>
</div>

---

*Source: `VarOnl/BlAutoLayout.htm`*
