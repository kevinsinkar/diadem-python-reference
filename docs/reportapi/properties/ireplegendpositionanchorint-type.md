---
title: "IRepLegendPositionAnchorInt.Type"
description: "Specifies in DIAdem REPORT whether the legend of an axis system is bound to an axis system, or whether you can position it freely. When the legend is bound to a"
---

# IRepLegendPositionAnchorInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for LegendPositionAnchor

Specifies in DIAdem REPORT whether the legend of an axis system is bound to an axis system, or whether you can position it freely. When the legend is bound to an axis system, DIAdem also moves the legend when you move the axis system.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendAnchorTypePageRelated` | 0 | Position freely |
| `eLegendAnchorTypeSystemRelated` | 1 | Bound to axis system |

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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepLegendPositionAnchorInt.htm`*
