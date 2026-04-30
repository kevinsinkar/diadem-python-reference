---
title: "IRepCurveLegendSettingsInt.UseAutoFontSize"
description: "Specifies whether DIAdem REPORT determines the font size of the legend label in an axis system automatically."
---

# IRepCurveLegendSettingsInt.UseAutoFontSize

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseAutoFontSize for CurveLegendSettings

Specifies whether DIAdem REPORT determines the font size of the legend label in an axis system automatically.

## Signature

```python
obj.UseAutoFontSize
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
oMyLegend.Settings.UseAutoFontSize = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseAutoFontSize_IRepCurveLegendSettingsInt.htm`*
