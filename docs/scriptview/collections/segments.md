---
title: "Segments"
description: "The Segments object provides a collection of the Segments in a channel table in DIAdem VIEW. Use the Segments collection to delete segment items or to add new s"
---

# Segments

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: Segments

The Segments object provides a collection of the Segments in a channel table in DIAdem VIEW. Use the Segments collection to delete segment items or to add new segments.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples/Data/Segment.tdm")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMySegment = oMyChart.Segments.Add("[1]/[3]", "[1]/[4]", "X")
oMySegment.Color = "grey"
oMySegment.Transparency = 50
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itosegmentenumint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itosegmentenumint-add/">Add</a> | <a href="../../methods/itosegmentenumint-item/">Item</a> | <a href="../../methods/itosegmentenumint-remove/">Remove</a> | <a href="../../methods/itosegmentenumint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ito2dchartint/">CurveChart2D</a>.<a href="../../properties/ito2dchartint-segments/">Segments</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToSegmentEnumInt.htm`*
