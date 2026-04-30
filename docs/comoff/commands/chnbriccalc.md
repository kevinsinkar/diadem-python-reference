---
title: "ChnBrICCalc"
description: "Calculates the Rational Brain Injury Criterion values (BrIC). The BRIC value estimates the injury risk of the brain due to rotary movements of the skull."
---

# ChnBrICCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnBrICCalc

Calculates the Rational Brain Injury Criterion values (BrIC). The BRIC value estimates the injury risk of the brain due to rotary movements of the skull.

## Signature

```python
dd.ChnBrICCalc( X , Y , Z )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which differs from the DIAdem version, in the following custom properties of the input channel: <span class="Monospace">ResultBrIC</span> and <span class="Monospace">ResultBrICVersion</span>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">BrIC criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel that contains the x-values of the signal in rad/s (angular velocity).</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal in rad/s (angular velocity).</td></tr>
<tr><td width="150"><em>Z</em></td>
<td>Specifies the data channel that contains the y-values of the signal in rad/s (angular velocity).</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">BrIC</td><td>Receives the result of the BrIC calculation.<div id="exp_BrIC">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">BrICVersion</td><td>Receives the version number of the BrIC calculation routine.<div id="exp_BrICVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnBrICCalc.htm`*
