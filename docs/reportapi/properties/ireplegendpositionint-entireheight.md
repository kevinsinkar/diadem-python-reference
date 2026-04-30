---
title: "IRepLegendPositionInt.EntireHeight"
description: "Specifies the legend height as a percentage of the worksheet in an axis system in DIAdem REPORT."
---

# IRepLegendPositionInt.EntireHeight

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: EntireHeight for LegendPosition

Specifies the legend height as a percentage of the worksheet in an axis system in DIAdem REPORT.

## Signature

```python
obj.EntireHeight
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyLegendPosition = oMyLegend.Position
oMyLegendPosition.SizeMode = dd.eLegendSizeFixed
oMyLegendPosition.EntireWidth = 25
oMyLegendPosition.EntireHeight = 10
oLegendPositionAnchor = oMyLegendPosition.Anchor
oLegendPositionAnchor.PageRelatedX = 50
oLegendPositionAnchor.PageRelatedY = 15
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_EntireHeight_IRepLegendPositionInt.htm`*
