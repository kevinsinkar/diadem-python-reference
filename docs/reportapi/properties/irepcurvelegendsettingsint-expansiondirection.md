---
title: "IRepCurveLegendSettingsInt.ExpansionDirection"
description: "Specifies in which direction DIAdem REPORT structures the curve legend of an axis system."
---

# IRepCurveLegendSettingsInt.ExpansionDirection

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ExpansionDirection for CurveLegendSettings

Specifies in which direction DIAdem REPORT structures the curve legend of an axis system.

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
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyCurveLegend = oMy2DAxisSystem.CurveLegend
oMyCurveLegend.Visible = True
oMyCurveLegendSettings = oMyCurveLegend.Settings
oMyCurveLegendSettings.Font.Name = "Times Roman"()
oMyCurveLegendSettings.Font.Bold = True
oMyCurveLegendSettings.ExpansionDirection = dd.eLegendGrowthExpansionBottomUp
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ExpansionDirection_IRepCurveLegendSettingsInt.htm`*
