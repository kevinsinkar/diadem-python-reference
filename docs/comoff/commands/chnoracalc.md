---
title: "ChnORACalc"
description: "Calculates the Occupant Ridedown Acceleration (ORA)."
---

# ChnORACalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnORACalc

Calculates the Occupant Ridedown Acceleration (ORA).

## Signature

```python
dd.ChnORACalc( XW , X1 , Y1 , ORATime0)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which differs from the DIAdem version number, in the following custom properties of the input channel: <span class="Monospace">ResultORAMax</span>, <span class="Monospace">ResultORATime</span>, and <span class="Monospace">ResultORAVersion</span>.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the standard EN 1317-1, Road Restraint Systems, Part 1 Terminology and General Criteria for Test Methods, for more information about this crash function.</td>
</tr>
</table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the descriptions of the <a href="#" data-unresolved="1">Crash Analysis Criteria</a> for further information such as background, input values, and rules and regulations. </td></tr></table>
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
<tr><td width="150">ORATime0</td>
<td>Specifies the time of collision in seconds.<div id="exp_ORATime0">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ORATime0 &lt;= 1E300</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ORATime</td><td>Receives the time of the stoppage deceleration.<div id="exp_ORATime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ORAMax</td><td>Receives the stoppage deceleration after the impact in gn (gravity acceleration).<div id="exp_ORAMax">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ORAVersion</td><td>Receives the version number of the ORA calculation routine.<div id="exp_ORAVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnORACalc.htm`*
