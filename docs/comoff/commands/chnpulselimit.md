---
title: "ChnPulseLimit"
description: "Checks whether acceleration values are in a specified range."
---

# ChnPulseLimit

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnPulseLimit

Checks whether acceleration values are in a specified range.

## Signature

```python
dd.ChnPulseLimit( XW , Y , X1 , Y1 , X2 , Y2 )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which is independent of the DIAdem version, in the following custom properties of the input channel: <span class="Monospace">ResultPulseLimit</span>, <span class="Monospace">ResultPulseLimitTIdx</span>, and <span class="Monospace">ResultPulseLimitVersion</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The data channel that contains the time values must be strictly monotonic increasing. The data channels that contain the x-interpolation points must be monotonic increasing.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">Pulse Test</a> for further information such as background, input values, and rules and regulations. </td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds. If the associated y-channel is a waveform channel or an xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the acceleration values in gn (acceleration of gravity).</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel that contains the x-interpolation points of the upper limit curve.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel that contains the y-interpolation points of the upper limit curve.</td></tr>
<tr><td width="150"><em>X2</em></td>
<td>Specifies the data channel that contains the x-interpolation points of the lower limit curve.</td></tr>
<tr><td width="150"><em>Y2</em></td>
<td>Specifies the data channel that contains the y-interpolation points of the lower limit curve.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">PulseLimit</td><td>Specifies whether the measured value is entirely within the specified range.<div id="exp_PulseLimit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">PulseLimitTIdx</td><td>Receives the number of the first point outside the given range.<div id="exp_PulseLimitTIdx">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger Variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PulseLimitVer</td><td>Receives the version number of the pulse limit calculation routine.<div id="exp_PulseLimitVer">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnPulseLimit.htm`*
