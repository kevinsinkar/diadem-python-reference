---
title: "ChnSICalc"
description: "Calculates the Severity Index (SI) which is an injury criterion for the chest and rib area."
---

# ChnSICalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSICalc

Calculates the Severity Index (SI) which is an injury criterion for the chest and rib area.

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">SI criterion</a> for further information such as background, input values, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the result of the SI calculation. The return value is a SIcum type.<div id="exp_SIcum">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnSICalc.htm`*
