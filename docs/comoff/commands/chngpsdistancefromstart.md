---
title: "ChnGPSDistanceFromStart"
description: "Calculates the shortest distance of the first coordinate to the following coordinates considering the ellipsoidal shape of the Earth. The function sums up the v"
---

# ChnGPSDistanceFromStart

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnGPSDistanceFromStart

Calculates the shortest distance of the first coordinate to the following coordinates considering the ellipsoidal shape of the Earth. The function sums up the values.

## Signature

```python
return_value = dd.ChnGPSDistanceFromStart( Y , Y1 , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the channel with the latitudes in °. Valid values are between <span class="Monospace">-90.0°</span> and <span class="Monospace">+90.0°</span>.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the channel with the longitudes in °. Valid values are between <span class="Monospace">-180.0°</span> and <span class="Monospace">+180.0°</span>.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel. The channel contains the running sum of the distances in <span class="Monospace">m</span> (meters).</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel with the difference values. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnGPSDistanceFromStart.htm`*
