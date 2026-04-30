---
title: "IRepCurveLegendSettingsInt.Font"
description: "Specifies the properties of the curve legend font in an axis system in DIAdem REPORT."
---

# IRepCurveLegendSettingsInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for CurveLegendSettings

Specifies the properties of the curve legend font in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
```

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
oMyCurveLegend.Settings.Font.Name = "Times Roman"()
oMyCurveLegend.Settings.Font.Bold = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepCurveLegendSettingsInt.htm`*
