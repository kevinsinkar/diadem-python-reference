---
title: "IRepLegendPositionInt.Anchor"
description: "Specifies the properties of the legend position in an axis system in DIAdem REPORT."
---

# IRepLegendPositionInt.Anchor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Anchor for LegendPosition

Specifies the properties of the legend position in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Anchor
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
oMyAnchor.Type = dd.eLegendAnchorTypePageRelated
oMyAnchor.PageRelatedX = 10
oMyAnchor.PageRelatedY = 10
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Anchor_IRepLegendPositionInt.htm`*
