---
title: "IRepCurveLegendSettingsInt.BackgroundColor"
description: "Specifies the background color of the curve legend in DIAdem REPORT."
---

# IRepCurveLegendSettingsInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for CurveLegendSettings

Specifies the background color of the curve legend in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyLegend.Settings.BackgroundColor.SetPredefinedColor(dd.eColorIndexGrey)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepCurveLegendSettingsInt.htm`*
