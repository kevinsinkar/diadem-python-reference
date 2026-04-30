---
title: "IRepCurveLegendSettingsInt.Angle"
description: "Specifies at which angle DIAdem REPORT displays the curve legend of an axis system."
---

# IRepCurveLegendSettingsInt.Angle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Angle for ColorLegendSettings

Specifies at which angle DIAdem REPORT displays the curve legend of an axis system.

## Signature

```python
obj.Angle
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAngle0` | 0 |  |
| `eAngle090` | 1 | 90 |
| `eAngle180` | 2 | 180 |
| `eAngle270` | 3 | 270 |

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
oMyCurveLegendSettings.Angle = dd.eAngle0
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Angle_IRepCurveLegendSettingsInt.htm`*
