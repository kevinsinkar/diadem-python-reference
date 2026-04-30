---
title: "ChnTHIVCalc"
description: "Calculates the Theoretical Head Impact Velocity (THIV)."
---

# ChnTHIVCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnTHIVCalc

Calculates the Theoretical Head Impact Velocity (THIV).

## Signature

```python
return_value = dd.ChnTHIVCalc( XW , Y , X1 , Y1 , THIVAngle, THIVDistanceX0, THIVDeltaX, THIVDeltaY, ResultChannel , ResultChannel , [THIVDistanceY0])
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which differs from the DIAdem version number, in the following custom properties of the input channel: <span class="Monospace">ResultPHDTime0</span>, <span class="Monospace">ResultTHIVFlailSpace</span>, <span class="Monospace">ResultTHIVTimeFlight</span>, <span class="Monospace">ResultTHIVVelocity</span>, and <span class="Monospace">ResultTHIVVersion</span>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the descriptions of the <a href="#" data-unresolved="1">Crash Analysis Criteria</a> for further information such as background, input values, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds. If all other channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the rotational velocity in radians per second.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel that contains the x-acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel that contains the y-acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150">THIVAngle</td>
<td>Specifies the angle between the direction of the vehicle and the vehicle axis at the time of impact, in radians.<div id="exp_THIVAngle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= THIVAngle &lt;= 2</td></tr>
</table>
</div></td></tr>
<tr><td width="150">THIVDistanceX0</td>
<td>Specifies the distance between the theoretical head and the center of gravity in x-direction in meters.<div id="exp_THIVDistanceX0">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>-5 &lt;= THIVDistanceX0 &lt;= 5</td></tr>
</table>
</div></td></tr>
<tr><td width="150">THIVDeltaX</td>
<td>Specifies the distance between the theoretical head and the theoretical impact surface in x-direction in meters.<div id="exp_THIVDeltaX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= THIVDeltaX &lt;= 3</td></tr>
</table>
</div></td></tr>
<tr><td width="150">THIVDeltaY</td>
<td>Specifies the distance between the theoretical head and the theoretical impact surface in y-direction in meters.<div id="exp_THIVDeltaY">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= THIVDeltaY &lt;= 3</td></tr>
</table>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel. The channel receives the time values up to the collision of the theoretical head with the theoretical impact surface, in seconds.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel. The channel receives the impact velocity of the theoretical head in kilometers per hour associated with the values of the <span class="Monospace">TimeOfFlight</span> channel.</td></tr>
<tr><td width="150">[THIVDistanceY0]</td>
<td>Specifies the distance between the theoretical head and the vehicle center of gravity in meters at the time of the impact.<div id="exp_THIVDistanceY0">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>-5 &lt;= THIVDistanceY0 &lt;= 5</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels. The first channel receives the time values up to the collision of the theoretical head with the theoretical impact surface in seconds, and the second channel receives the impact velocities of the theoretical head which belong to the values of the <span class="Monospace">TimeOfFlight</span> channel in kilometers per hour. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyX1Channel = dd.Data.Root.ChannelGroups(2).Channels(3)
oMyY1Channel = dd.Data.Root.ChannelGroups(2).Channels(4)
oMyResultChn = dd.ChnTHIVCalc(oMyXChannel, oMyYChannel, oMyX1Channel, oMyY1Channel, 0, 0, 0.6, 0.3, "Results/TimeOfFlight", "Results/THIV", 0)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
oMyResultChn = dd.ChnTHIVCalc("[2]/[1]","[2]/[2]", "[2]/[3]","[2]/[4]", 0, 0, 0.6, 0.3, "Result/TimeOfFlight", "Result/THIV", 0)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnTHIVCalc.htm`*
