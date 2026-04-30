---
title: "ChnFFCCalc"
description: "Calculates the Femur Force Criterion values (FFC), which is the force on the femur."
---

# ChnFFCCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFFCCalc

Calculates the Femur Force Criterion values (FFC), which is the force on the femur.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The input channels must be filtered with CFC600.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">FFC criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the force in newtons.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the load duration in seconds.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the amplitudes in newtons.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the injury probability.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the version number of the FFC calculation routine. The return value is a FFCVersion type.<div id="exp_FFCVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnFFCCalc.htm`*
