---
title: "IRepD2SegmentInt"
description: "The 2DBackgroundSegment object provides the background segment of a 2D axis system in DIAdem REPORT."
---

# IRepD2SegmentInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBackgroundSegment

The 2DBackgroundSegment object provides the background segment of a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "examples\\data\\Segment.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMySegement = oMy2DAxisSystem.Settings.BackgroundSegments.Add()
oMySegement.Color.SetPredefinedColor(dd.eColorIndexYellow)
oMySegement.XChannel.Reference = "[1]/[3]"
oMySegement.YChannel.Reference = "[1]/[4]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2segmentint-color/">Color</a> | <a href="../../properties/irepd2segmentint-orientation/">Orientation</a> | <a href="../../properties/irepd2segmentint-xchannel/">XChannel</a> | <a href="../../properties/irepd2segmentint-ychannel/">YChannel</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dbackgroundsegments/">2DBackgroundSegments</a>.<a href="../../methods/irepd2segmentlistint-add/">Add</a> | <a href="../../collections/2dbackgroundsegments/">2DBackgroundSegments</a>.<a href="../../methods/irepd2segmentlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2SegmentInt.htm`*
