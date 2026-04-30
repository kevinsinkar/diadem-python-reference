---
title: "IRepLegendPositionInt.InteractiveMoveMode"
description: "Specifies whether DIAdem REPORT moves the legend when you move the associated axis system."
---

# IRepLegendPositionInt.InteractiveMoveMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: InteractiveMoveMode for LegendPosition

Specifies whether DIAdem REPORT moves the legend when you move the associated axis system.

## Signature

```python
obj.InteractiveMoveMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendMoveAutomatic` | 0 | Automatic—DIAdem automatically determines whether to move the legend when you move the axis system, depending on the legend position. If the legend is completely outside the axis system, you can move the axis system without DIAdem moving the legend simultaneously. |
| `eLegendMoveWithAxisSystem` | 1 | Bound to axis system—DIAdem moves the legend as soon as you move the respective axis system. |
| `eLegendMoveIndependent` | 2 | Free—DIAdem does not move the legend when you move the respective axis system. |

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
oMyLegendPosition.InteractiveMoveMode = dd.eLegendMoveAutomatic
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

*Source: `ReportApi/properties/Report_property_InteractiveMoveMode_IRepLegendPositionInt.htm`*
