---
title: "CircleRegrCalc"
description: "Calculates the regression circle for a set of points."
---

# CircleRegrCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: CircleRegrCalc

Calculates the regression circle for a set of points.

## Signature

```python
return_value = dd.CircleRegrCalc( XW , Y , ResultChannel , ResultChannel , CircleResol)
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
<td>Specifies the data channel that contains the x-coordinates of the point set. If the y-channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-coordinates of the point set.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-coordinates of the regression circle.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-coordinates of the regression circle.</td></tr>
<tr><td width="150">CircleResol</td>
<td>Specifies the number of points per approximation circle.<div id="exp_CircleResol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>3 &lt;= CircleResol &lt;= 65535</td></tr>
</table>
<p class="Body">DIAdem uses a circle approximation with various approximation procedures to calculate regression circles, envelope circles, and fitting incircles for a specified set of points. The <span class="Monospace">CircleResol</span> variable specifies the resolution of the circles to be calculated. The circle resolution specifies the number of points per approximation circle. To obtain a closed circle during approximation, DIAdem generates an additional point that corresponds to the first point in the approximation circle. Therefore the channels where DIAdem saves the coordinates of the approximation circle are one value longer than the circle resolution.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/CircleRegrCalc.htm`*
