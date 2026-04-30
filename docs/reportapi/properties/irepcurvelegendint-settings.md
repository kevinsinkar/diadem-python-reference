---
title: "IRepCurveLegendInt.Settings"
description: "Specifies the properties of a legend in an axis system in DIAdem REPORT."
---

# IRepCurveLegendInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for CurveLegend

Specifies the properties of a legend in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
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
oMyCurveLegend.Settings.Orientation = dd.eLegendOrientationVertical
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepCurveLegendInt.htm`*
