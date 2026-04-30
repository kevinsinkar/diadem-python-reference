---
title: "BlLimit2ColorRGB"
description: "Specifies the RGB values for the color of the alarm range in display instruments."
---

# BlLimit2ColorRGB

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlLimit2ColorRGB

Specifies the RGB values for the color of the alarm range in display instruments.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlLimit2ColorRGB = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless" id="table6">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note</strong>  Refer to the <a href="#" data-unresolved="1">RGB function</a> description for more information about the red, green, and blue color values.</td>
</tr>
</table>
<table class="Borderless" id="table7">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note  </strong>To assign a value to the <span class="Monospace">BlLimit2ColorRGB</span> variable, you must first assign the value <span class="Monospace">other colors</span> to the <a href="../bllimit2color/">BlLimit2Color</a> variable.</td>
</tr>
</table>
</div>

---

*Source: `VarOnl/BlLimit2ColorRGB.htm`*
