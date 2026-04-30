---
title: "ChnTICalc"
description: "Calculates the Tibia Index value (TI). This value is an injury criterion for the lower leg."
---

# ChnTICalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnTICalc

Calculates the Tibia Index value (TI). This value is an injury criterion for the lower leg.

## Signature

```python
dd.ChnTICalc( XW , Y , Y1 , Y2 , TIMcR, TIFcZ)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which differs from the DIAdem version number, in the following custom properties of the input channel: <span class="Monospace">ResultTIResult</span>, <span class="Monospace">ResultTITime</span>, and <span class="Monospace">ResultTIVersion</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The input channels must be filtered with CFC600.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">TI criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the bending moment around the x-axis in newton meters.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel that contains the bending moment around the y-axis in newton meters.</td></tr>
<tr><td width="150"><em>Y2</em></td>
<td>Specifies the data channel that contains the axial compression force in the z-direction in kilonewtons.</td></tr>
<tr><td width="150">TIMcR</td>
<td>Specifies the critical bending moment Mc in newton meters.<div id="exp_TIMcR">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">TIFcZ</td>
<td>Specifies the critical compression force Fc in the z-direction, in kilonewtons.<div id="exp_TIFcZ">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">TIRes</td><td>Receives the result of the TI calculation.<div id="exp_TIRes">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">TIVersion</td><td>Receives the version number of the Tibia Index calculation routine.<div id="exp_TIVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">TITime</td><td>Receives the moment of the calculated Tibia index in seconds.<div id="exp_TITime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnTICalc.htm`*
