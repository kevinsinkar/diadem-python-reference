---
title: "ChnLinGenImp"
description: "Generates an implicit channel with a prescribed linear generation."
---

# ChnLinGenImp

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnLinGenImp

Generates an implicit channel with a prescribed linear generation.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not enter a channel name, DIAdem generates a channel name.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem uses the start value and the difference between two successive values to define implicit channels. When saving implicit channels, DIAdem only saves the parameters of the generation specifications.<br attr="ext"/>DIAdem always creates a new channel in the default group. If the name does not conform to the <a href="#" data-unresolved="1">name conventions</a>, DIAdem corrects the name. If there is already a channel with this name, DIAdem adds a number to the valid name.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">GHdChnName</td>
<td>Specifies the name suggestion for a channel in the Data Portal.<div id="exp_GHdChnName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you do not enter a channel name, DIAdem generates a channel name.</td></tr></table>
</div></td></tr>
<tr><td width="150">GHdChnLength</td>
<td>Specifies the maximum number of values per channel. The default value of the <span class="Monospace">GHdChnLength</span> variable is <span class="Monospace">0</span>.<div id="exp_GHdChnLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= GHdChnLength &lt;= 2147483647</td></tr>
</table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">GHdStartVal</td>
<td>Specifies the first value of implicit data channels and the offset of explicit data channels.<div id="exp_GHdStartVal">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">In implicit data channels the <span class="Monospace">GHdStartVal</span> variable specifies the first channel value. DIAdem adds a constant step width to the first channel value to generate the other channel values.</p>
<p class="Body">If the data channels are explicit, the variable <span class="Monospace">GHdStartVal</span> specifies the offset that DIAdem adds to the explicit channel values when they are read in. Together with the step width DIAdem calibrates the data when the data is read in.</p>
</div></td></tr>
<tr><td width="150">GHdStep</td>
<td>Specifies the difference between two successive values.<div id="exp_GHdStep">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[GenXUnitPreset]</td>
<td>Specifies the unit in which DIAdem generates the numeric channel. By default DIAdem does not use a unit. <div id="exp_GenXUnitPreset">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">String variable</a> type. Receives the name of the new channel.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnLinGenImp.htm`*
