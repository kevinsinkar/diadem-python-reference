---
title: "IRepD2SegmentInt.Orientation"
description: "Specifies the alignment of the segments a 2D axis system in DIAdem REPORT."
---

# IRepD2SegmentInt.Orientation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Orientation for 2DBackgroundSegment

Specifies the alignment of the segments a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Orientation
```

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
oMySegement.Color.SetPredefinedColor(dd.eColorIndexGrey)
oMySegement.XChannel.Reference = "[1]/[3]"
oMySegement.YChannel.Reference = "[1]/[4]"
oMySegement.Orientation = dd.e2DSegmentOrientationX
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Orientation_IRepD2SegmentInt.htm`*
