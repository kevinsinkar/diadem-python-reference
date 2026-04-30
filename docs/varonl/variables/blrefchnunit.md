---
title: "BlRefChnUnit"
description: "Specifies the unit of the reference channel or the time channel that DIAdem creates when DIAdem saves measurement values."
---

# BlRefChnUnit

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlRefChnUnit

Specifies the unit of the reference channel or the time channel that DIAdem creates when DIAdem saves measurement values.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    BlRefChnUnit = <em>Value</em>
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>For more information, refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you set <span class="Monospace">absolute time</span>, the maximum resolution is <span class="Monospace">1</span> second.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>When measuring in the <a href="#" data-unresolved="1">Hardware clock</a>, use the settings <span class="Monospace">run. number</span>, <span class="Monospace">seconds</span>, or <span class="Monospace">milliseconds</span> for the time channel because DIAdem does need start times for these settings. DIAdem specifies the start times during the measurement. DIAdem cannot specify precise start times because signal processing with hardware clock is fast or asynchronous. Therefore, two clock systems that use the same start trigger do not always start with the same time value.</td></tr></table>
</div>

---

*Source: `VarOnl/BlRefChnUnit.htm`*
