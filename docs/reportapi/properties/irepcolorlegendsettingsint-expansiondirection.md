---
title: "IRepColorLegendSettingsInt.ExpansionDirection"
description: "Specifies in which direction DIAdem REPORT structures the color legend of an axis system."
---

# IRepColorLegendSettingsInt.ExpansionDirection

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ExpansionDirection for ColorLegendSettings

Specifies in which direction DIAdem REPORT structures the color legend of an axis system.

## Signature

```python
obj.ExpansionDirection
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendGrowthExpansionTopDown` | 0 | From top down |
| `eLegendGrowthExpansionBottomUp` | 1 | From bottom up |

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
oMyColorLegend.Settings.ExpansionDirection = dd.eLegendGrowthExpansionTopDown
oMyNumbers = oMyColorLegend.Settings.Numbers
oMyNumbers.Format = "d.ddde"
oMyNumbers.Mode = dd.eColorLegendScaleSingleValue
oMyNumbers.ValueMode = dd.eColorLegendScaleValueModeCenter
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ExpansionDirection_IRepColorLegendSettingsInt.htm`*
