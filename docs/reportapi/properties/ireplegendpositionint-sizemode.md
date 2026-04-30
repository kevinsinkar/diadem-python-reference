---
title: "IRepLegendPositionInt.SizeMode"
description: "Specifies whether DIAdem REPORT specifies the height and width of the legend of an axis system for individual elements or for the entire legend."
---

# IRepLegendPositionInt.SizeMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SizeMode for LegendPosition

Specifies whether DIAdem REPORT specifies the height and width of the legend of an axis system for individual elements or for the entire legend.

## Signature

```python
obj.SizeMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendSizeFixed` | 0 | The number of legend entries does not impact the legend size. |
| `eLegendSizeElementwise` | 1 | DIAdem adjusts the legend size to the number of legend entries. |

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
oMyLegendPositionAnchor.PageRelatedY = 11
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SizeMode_IRepLegendPositionInt.htm`*
