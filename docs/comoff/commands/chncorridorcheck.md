---
title: "ChnCorridorCheck"
description: "Checks whether a signal is in a specified range."
---

# ChnCorridorCheck

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnCorridorCheck

Checks whether a signal is in a specified range.

## Signature

```python
dd.ChnCorridorCheck( XW , Y , X1 , Y1 , X2 , Y2 )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  DIAdem saves the calculation results and the version number of the algorithm which is not the same as the DIAdem version number in the following custom properties of the input channel: <span class="Monospace">Result~CorridorCheck</span>, <span class="Monospace">Result~CorridorCheck~TIdx</span>, and <span class="Monospace">Result~CorridorCheck~Version</span>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">Pulse Test</a> for further information such as background, input values, and rules and regulations. </td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values. If the associated y-channel is a waveform or xy-channel, you do not need to specify this channel. The data channel that contains the x-values must be strictly monotonic increasing.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel that contains the x-interpolation points of the upper limit curve. You must also specify this channel if the associated y1-channel is a waveform channel. The data channels that contain the x-interpolation points must be monotonic increasing.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel that contains the y-interpolation points of the upper limit curve.</td></tr>
<tr><td width="150"><em>X2</em></td>
<td>Specifies the data channel that contains the x-interpolation points of the lower limit curve. You must also specify this channel if the associated y2-channel is a waveform channel. The data channels that contain the x-interpolation points must be monotonic increasing.</td></tr>
<tr><td width="150"><em>Y2</em></td>
<td>Specifies the data channel that contains the y-interpolation points of the lower limit curve.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CorridorCheck</td><td>Specifies whether the signal is entirely within the specified range.<div id="exp_CorridorCheck">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">CorridorCheckTIdx</td><td>Receives the number of the first point outside the given range.<div id="exp_CorridorCheckTIdx">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">CorridorCheckVersion</td><td>Receives the version number of the CorridorCheck calculation routine.<div id="exp_CorridorCheckVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnCorridorCheck.htm`*
