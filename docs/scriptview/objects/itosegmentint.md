---
title: "IToSegmentInt"
description: "The Segment object provides access to a segment in a 2D axis system in DIAdem VIEW. Use the Segment object to specify the segment properties."
---

# IToSegmentInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Segment

The Segment object provides access to a segment in a 2D axis system in DIAdem VIEW. Use the Segment object to specify the segment properties.

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
<p><a href="../../properties/itosegmentint-color/">Color</a> | <a href="../../properties/itosegmentint-colorrgb/">ColorRGB</a> | <a href="../../properties/itosegmentint-direction/">Direction</a> | <a href="../../properties/itosegmentint-index/">Index</a> | <a href="../../properties/itosegmentint-name/">Name</a> | <a href="../../properties/itosegmentint-tagstored/">TagStored</a> | <a href="../../properties/itosegmentint-tagtemporary/">TagTemporary</a> | <a href="../../properties/itosegmentint-transparency/">Transparency</a> | <a href="../../properties/itosegmentint-xchannelname/">XChannelName</a> | <a href="../../properties/itosegmentint-ychannelname/">YChannelName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/segments/">Segments</a>.<a href="../../methods/itosegmentenumint-add/">Add</a> | <a href="../../collections/segments/">Segments</a>.<a href="../../methods/itosegmentenumint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToSegmentInt.htm`*
