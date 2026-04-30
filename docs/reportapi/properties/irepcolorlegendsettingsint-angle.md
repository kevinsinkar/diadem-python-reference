---
title: "IRepColorLegendSettingsInt.Angle"
description: "Specifies at which angle DIAdem REPORT displays the color legend of a curve."
---

# IRepColorLegendSettingsInt.Angle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Angle for ColorLegendSettings

Specifies at which angle DIAdem REPORT displays the color legend of a curve.

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
oMyColorLegend.Settings.Angle = dd.eAngle0
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

*Source: `ReportApi/properties/Report_property_Angle_IRepColorLegendSettingsInt.htm`*
