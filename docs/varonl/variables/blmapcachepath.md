---
title: "BlMapCachePath"
description: "Specifies the folder and its path which buffers maps from the map display."
---

# BlMapCachePath

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlMapCachePath

Specifies the folder and its path which buffers maps from the map display.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlMapCachePath = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>You can only save the current map data in a cache if you set the value of the <a href="../blmapcachetiles/">BlMapCacheTiles</a> variable to <span class="Monospace">TRUE</span>.</td></tr></table>
</div>

---

*Source: `VarOnl/BlMapCachePath.htm`*
