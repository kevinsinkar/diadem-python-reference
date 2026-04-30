---
title: "ChnNConvexHull"
description: "Calculates the non-convex hull of a set of points."
---

# ChnNConvexHull

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnNConvexHull

Calculates the non-convex hull of a set of points.

## Signature

```python
return_value = dd.ChnNConvexHull( X , Y , ResultChannel , ResultChannel , HullTol, HullFactor)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The value of the variable <span class="Monospace">HullFactor</span> should not be greater than the value of the variable <a href="../../../varoff/variables/hulltol/">HullTol</a> that specifies the maximum edge length of the hull.</td></tr></table>
</div>

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
<tr><td width="150">HullTol</td>
<td>When DIAdem calculates a non-convex hull, this variable specifies the maximum length of any edge of the hull as a percentage of the cross section of the set of points.<div id="exp_HullTol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= HullTol &lt;= 100</td></tr>
</table>
<p class="Body">To calculate a non-convex hull, DIAdem first determines the convex hull of the points. Then DIAdem searches for points near the edge for each each side of the convex hull. If DIAdem finds an edge with neighboring points, DIAdem divides this edge into two new edges if the edge is longer than the maximum length specified by the <span class="Monospace">HullTol</span> variable and if at least one of the new edges is shorter than the old edge. DIAdem only divides an edge that is shorter than the maximum length if other points are on it or close to it.</p>
<p class="Body">When DIAdem calculates the edges of the convex hull to the non-convex hull, DIAdem uses the longest edges first and the shortest edges last. This sequence can cause edges calculated later to exceed the maximum length specified in the <span class="Monospace">HullTol</span> variable because these edges need points that are already in the convex hull. Except for the start point each point is in the hull only once to prevent the hull from intersecting itself.</p>
</div></td></tr>
<tr><td width="150">HullFactor</td>
<td>In a non-convex hull calculation, this specifies the factor by which the new edge can be longer than the old edge.<div id="exp_HullFactor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>1 &lt;= HullFactor &lt;= 10</td></tr>
</table>
<p class="Body">When DIAdem calculates a non-convex hull, DIAdem extends the convex hull inwards by dividing one edge of the convex hull into two new edges. The <span class="Monospace">HullFactor</span> variable specifies how much longer the old edge may be versus the new edge. DIAdem can only subdivide an edge if at least one of the two new edges is shorter than the edge of the convex hull multiplied by the multiplication factor.</p>
<pre><donottranslate>Length(NewBorder) &lt; HullFactor * Length(OldBorder)</donottranslate></pre>
<p class="Body">If you assign the value <span class="Monospace">1</span> to the <span class="Monospace">HullFactor</span> variable, at least one of the two found edges is shorter than the original edge. Only assign a value greater than <span class="Monospace">1</span> to the <span class="Monospace">HullFactor</span> variable if DIAdem cannot achieve the desired difference in any other way.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  The value of the variable <span class="Monospace">HullFactor</span> should not be greater than the value of the variable <a href="../../../varoff/variables/hulltol/">HullTol</a> that specifies the maximum edge length of the hull.</td></tr></table>
</div></td></tr>
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
oMyResultChn = dd.ChnNConvexHull(oMyXChannel, oMyYChannel, "Results/NonConvexHullX", "Results/NonConvexHullY", 10, 1)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
oMyResultChn = dd.ChnNConvexHull("[1]/[1]", "[1]/[2]", "Results/NonConvexHullX", "Results/NonConvexHullY", 10, 1)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnNConvexHull.htm`*
