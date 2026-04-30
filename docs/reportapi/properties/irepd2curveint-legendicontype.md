---
title: "IRepD2CurveInt.LegendIconType"
description: "Specifies the display of the legend symbols in a 2D axis system in DIAdem REPORT."
---

# IRepD2CurveInt.LegendIconType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LegendIconType for 2DCurve

Specifies the display of the legend symbols in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.LegendIconType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendIconAllCurveStyles` | 0 | Complete |
| `eLegendIconBasicCurveStylesOnly` | 1 | Only display type |
| `eLegendIconExtendedCurveStylesOnly` | 2 | Only extensions |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMy2DCurve.Shape.Extensions.Marker.Type = dd.eMarkerCross
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMy2DCurve.LegendIconType = dd.eLegendIconAllCurveStyles
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LegendIconType_IRepD2CurveInt.htm`*
