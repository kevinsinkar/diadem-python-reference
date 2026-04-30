---
title: "ChnConvexHull"
description: "Calculates the convex hull of a set of points."
---

# ChnConvexHull

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvexHull

Calculates the convex hull of a set of points.

## Signature

```python
return_value = dd.ChnConvexHull( X , Y , ResultChannel , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values of the point set.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the points.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-values of the hull.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the hull.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains two result channels. The first result channel contains the x-values and the second result channel contains the y-values of the hull. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyResultChn = dd.ChnConvexHull(oMyXChannel, oMyYChannel, "Results/ConvexHullX", "Results/ConvexHullY")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
oMyResultChn = dd.ChnConvexHull("[1]/[1]", "[1]/[2]", "Results/ConvexHullX", "Results/ConvexHullY")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnConvexHull.htm`*
