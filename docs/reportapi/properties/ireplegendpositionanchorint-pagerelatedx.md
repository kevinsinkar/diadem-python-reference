---
title: "IRepLegendPositionAnchorInt.PageRelatedX"
description: "Specifies the distance between the reference point of the legend of an axis system and the left edge of the worksheet as a percentage of the width of the worksh"
---

# IRepLegendPositionAnchorInt.PageRelatedX

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PageRelatedX for LegendPositionAnchor

Specifies the distance between the reference point of the legend of an axis system and the left edge of the worksheet as a percentage of the width of the worksheet in DIAdem REPORT.

## Signature

```python
obj.PageRelatedX
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
oMyAnchor = oMyLegend.Position.Anchor
oMyAnchor.PageRelatedX = 10
oMyAnchor.PageRelatedY = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PageRelatedX_IRepLegendPositionAnchorInt.htm`*
