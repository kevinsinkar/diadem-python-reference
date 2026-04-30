---
title: "ChnOIVCalc"
description: "Calculates the Occupant Impact Velocity (OIV)."
---

# ChnOIVCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnOIVCalc

Calculates the Occupant Impact Velocity (OIV).

## Signature

```python
dd.ChnOIVCalc( XW , X1 , Y1 , OIVDistance, OIVDeltaX, OIVDeltaY)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the calculated results and the version number, which is independent of the DIAdem version, in the following custom properties of the input channel: <span class="Monospace">ResultOIVTimeFlight</span>, <span class="Monospace">ResultOIVVelocity</span>, and <span class="Monospace">ResultOIVVersion</span>.</td></tr></table>
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
<tr><td width="150">OIVDistance</td>
<td>Specifies the distance between the theoretical head and the vehicle center of gravity in meters.<div id="exp_OIVDistance">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>-5 &lt;= OIVDistance &lt;= 5</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OIVDeltaX</td>
<td>Specifies the distance between the theoretical head and the theoretical impact surface in x-direction in meters.<div id="exp_OIVDeltaX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= OIVDeltaX &lt;= 3</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OIVDeltaY</td>
<td>Specifies the distance between the theoretical head and the theoretical impact surface in y-direction in meters.<div id="exp_OIVDeltaY">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= OIVDeltaY &lt;= 3</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OIVTimeFlight</td><td>Receives the period of time in seconds during which the impact moves the passengers.<div id="exp_OIVTimeFlight">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">OIVVelocity</td><td>Receives the impact velocity of the passengers in kilometers per hour.<div id="exp_OIVVelocity">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">OIVVersion</td><td>Receives the version number of the OIV calculation routine.<div id="exp_OIVVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnOIVCalc.htm`*
