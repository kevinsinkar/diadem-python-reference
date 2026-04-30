---
title: "IRepCurveLegendSettingsInt.UseTextClipping"
description: "Specifies whether DIAdem REPORT truncates the legend label of an axis system at the edge of the legend column. You must assign the value FALSE to the UseAutoFon"
---

# IRepCurveLegendSettingsInt.UseTextClipping

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseTextClipping for CurveLegendSettings

Specifies whether DIAdem REPORT truncates the legend label of an axis system at the edge of the legend column. You must assign the value FALSE to the UseAutoFontSize property in order to use the UseTextClipping property.

## Signature

```python
obj.UseTextClipping
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
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyLegend.Settings.UseAutoFontSize = False
oMyLegend.Settings.Font.Size = 6
oMyLegend.Settings.UseTextClipping = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseTextClipping_IRepCurveLegendSettingsInt.htm`*
