---
title: "ChnPHDCalc"
description: "Calculates the Post Impact Head Deceleration (PHD)."
---

# ChnPHDCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnPHDCalc

Calculates the Post Impact Head Deceleration (PHD).

## Signature

```python
dd.ChnPHDCalc( XW , X1 , Y1 , PHDTime0)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which differs from the DIAdem version number, in the following custom properties of the input channel: <span class="Monospace">ResultPHDMax</span>, <span class="Monospace">ResultPHDTime</span>, and <span class="Monospace">ResultPHDVersion</span>.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the standard EN 1317-1, Road Restraint Systems, Part 1 Terminology and General Criteria for Test Methods, for more information about this crash function.</td>
</tr>
</table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the descriptions of the <a href="#" data-unresolved="1">Crash Analysis Criteria</a> for further information such as background, input values, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values in seconds.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel that contains the x-acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel that contains the y-acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150">PHDTime0</td>
<td>Specifies the time of collision of the theoretical head with the theoretical impact surface, in seconds.<div id="exp_PHDTime0">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= PHDTime0 &lt;= 1E300</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">PHDTime</td><td>Receives the time for the maximum head delay, in seconds.<div id="exp_PHDTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PHDMax</td><td>Receives the maximum head deceleration after the impact in gn (acceleration of gravity).<div id="exp_PHDMax">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PHDVersion</td><td>Receives the version number of the PHD calculation routine.<div id="exp_PHDVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnPHDCalc.htm`*
