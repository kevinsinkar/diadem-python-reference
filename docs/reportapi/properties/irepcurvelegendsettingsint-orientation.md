---
title: "IRepCurveLegendSettingsInt.Orientation"
description: "Specifies the alignment of the legend in an axis system in DIAdem REPORT."
---

# IRepCurveLegendSettingsInt.Orientation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Orientation for CurveLegendSettings

Specifies the alignment of the legend in an axis system in DIAdem REPORT.

## Signature

```python
obj.Orientation
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendOrientationAutomatic` | 0 | Automatic—DIAdem aligns the legend vertically when the height/width ratio is greater than 0.7, otherwise the alignment is horizontal. |
| `eLegendOrientationHorizontal` | 1 | Horizontal—DIAdem positions the components of the legend next to each other and positions the labels below the respective component. |
| `eLegendOrientationVertical` | 2 | Vertical—DIAdem positions the components of the legend underneath each other and positions the labels next to the respective components. |

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
oMy2DAxisSystem.CurveLegend.Visible = True
oMy2DAxisSystem.CurveLegend.Settings.Orientation = dd.eLegendOrientationVertical
oMy2DAxisSystem.CurveLegend.Settings.BackgroundColor.SetPredefinedColor(dd.eColorIndexDarkViolet)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Orientation_IRepCurveLegendSettingsInt.htm`*
