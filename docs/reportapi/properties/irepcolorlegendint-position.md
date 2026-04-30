---
title: "IRepColorLegendInt.Position"
description: "Specifies the position of the color legend of an axis system in DIAdem REPORT."
---

# IRepColorLegendInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for ColorLegend

Specifies the position of the color legend of an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Position
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 10
oMyPos.X2 = 60
oMyPos.Y1 = 10
oMyPos.Y2 = 60
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColorLegend = oMy2DAxisSystem.ColorLegend
oMyColorLegend.Visible = True
oMyLegendPosition = oMyColorLegend.Position
oMyLegendPosition.SizeMode = dd.eLegendSizeFixed
oMyLegendPosition.EntireHeight = 30
oMyLegendPosition.EntireWidth = 20
oMyLegendPosition.InteractiveMoveMode = dd.eLegendMoveWithAxisSystem
oMyLegendPosition.RelativePosition = dd.eLegendRelativePositionBottomRight
oMyLegendPositionAnchor = oMyLegendPosition.Anchor
oMyLegendPositionAnchor.PageRelatedX = 92
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Position_IRepColorLegendInt.htm`*
