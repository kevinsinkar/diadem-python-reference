---
title: "IRepCurveLegendSettingsInt.ShowGridLines"
description: "Specifies whether DIAdem REPORT displays separators in the legend of an axis system."
---

# IRepCurveLegendSettingsInt.ShowGridLines

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowGridLines for CurveLegendSettings

Specifies whether DIAdem REPORT displays separators in the legend of an axis system.

## Signature

```python
obj.ShowGridLines
```

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve")
oMyShape = oMy2DCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyCurveLegend = oMy2DaxisSystem.CurveLegend
oMyCurveLegend.Visible = True
oMyCurveLegend.Columns.Add()
oMyCurveLegend.Settings.ShowGridLines = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowGridLines_IRepCurveLegendSettingsInt.htm`*
