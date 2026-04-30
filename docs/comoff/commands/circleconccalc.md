---
title: "CircleConcCalc"
description: "Calculates the regression circle, the concentric circumcircle, and the concentric incircle for a point set."
---

# CircleConcCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CircleConcCalc

Calculates the regression circle, the concentric circumcircle, and the concentric incircle for a point set.

## Signature

```python
return_value = dd.CircleConcCalc( XW , Y , ResultChannel , ResultChannel , ResultChannel , ResultChannel , ResultChannel , ResultChannel , CircleResol, CirclePrecision)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To calculate the circle approximation you need at least three points that are not collinear. DIAdem does not calculate with points that have a NoValue in at least one coordinate.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem adds one value to each result channel to achieve a closed circle. This value is the same as the first channel value. The channel length of the result channel is one value longer than the specified number of points in the approximation circle.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-coordinates of the point set. If the y-channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-coordinates of the point set.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-coordinates of the regression circle.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-coordinates of the regression circle.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-coordinates of the concentric circumcircle.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-coordinates of the concentric circumcircle.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-coordinates of the concentric incircle.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-coordinates of the concentric incircle.</td></tr>
<tr><td width="150">CircleResol</td>
<td>Specifies the number of points per approximation circle.<div id="exp_CircleResol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>3 &lt;= CircleResol &lt;= 65535</td></tr>
</table>
<p class="Body">DIAdem uses a circle approximation with various approximation procedures to calculate regression circles, envelope circles, and fitting incircles for a specified set of points. The <span class="Monospace">CircleResol</span> variable specifies the resolution of the circles to be calculated. The circle resolution specifies the number of points per approximation circle. To obtain a closed circle during approximation, DIAdem generates an additional point that corresponds to the first point in the approximation circle. Therefore the channels where DIAdem saves the coordinates of the approximation circle are one value longer than the circle resolution.</p>
</div></td></tr>
<tr><td width="150">CirclePrecision</td>
<td>Specifies the relative precision of the incircle and circumcircle calculation as a percentage of the radius of the regression circle.<div id="exp_CirclePrecision">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>1E-10 &lt;= CirclePrecision &lt;= 100</td></tr>
</table>
<p class="Body">DIAdem uses a circle approximation with various approximation procedures to calculate regression circles, envelope circles, and fitting incircles for a specified set of points. The procedures for calculating incircles and circumcircles are iterative. The result of each iteration step approaches the optimal solution. The <span class="Monospace">CirclePrecision</span> variable specifies a relative precision of the center point position. The relative precision data optimizes the turnaround time.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains six result channels with the x- and y-coordinates of the regression circle, and the concentric circumcircle and incircle. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyResultChn = dd.CircleConcCalc(oMyXChannel, oMyYChannel, "Results/RegressionCircleX", "Results/RegressionCircleY", "Results/ConcentricCircumCircleX", "Results/ConcentricCircumCircleY", "Results/ConcentricInCircleX", "Results/ConcentricInCircleY", 360, 0.01)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name , "\r\n" ,"Result channel(4): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(4).Name , "\r\n" ,"Result channel(5): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(5).Name , "\r\n" ,"Result channel(6): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(6).Name)
```

```python
oMyResultChn = dd.CircleConcCalc("[1]/[1]","[1]/[2]", "Results/RegressionCircleX", "Results/RegressionCircleY", "Results/ConcentricCircumCircleX", "Results/ConcentricCircumCircleY", "Results/ConcentricInCircleX", "Results/ConcentricInCircleY", 360, 0.01)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name , "\r\n" ,"Result channel(4): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(4).Name , "\r\n" ,"Result channel(5): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(5).Name , "\r\n" ,"Result channel(6): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(6).Name)
```

---

*Source: `ComOff/CircleConcCalc.htm`*
