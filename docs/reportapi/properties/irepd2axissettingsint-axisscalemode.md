---
title: "IRepD2AxisSettingsInt.AxisScaleMode"
description: "Specifies which method DIAdem uses to scale a 2D axis system in DIAdem REPORT. If you assign the value e2DAxisScalingModeForScaledOutput to the AxisScaleMode pr"
---

# IRepD2AxisSettingsInt.AxisScaleMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AxisScaleMode for 2DAxisSettings

Specifies which method DIAdem uses to scale a 2D axis system in DIAdem REPORT. If you assign the value e2DAxisScalingModeForScaledOutput to the AxisScaleMode property, DIAdem uses the given units per unit length for axis scaling. If, for example, you select 5 units per cm and you represent 60 units, the axis length is 12 cm. Since for automatic scaling DIAdem selects values such as 1, 2, 5, 10, 20, ... for the units per unit length, it is possible that DIAdem uses only part of the axis system to display the curve. If you assign the value e2DAxisScalingModeRangeOfValues to the AxisScaleMode property, DIAdem uses the entire value range of all displayed channels for scaling during automatic scaling. To display the curve, DIAdem uses the entire axis area. You cannot see from the scale settings how many units per unit length DIAdem uses for axis scaling.

## Signature

```python
obj.AxisScaleMode
```

## Python example

```python
dd.Report.NewLayout()
dd.Report.Settings.Page.Dimensions.UseScaledOutput = True
dd.Report.Settings.Page.Dimensions.SetPredefinedPageSize(dd.ePageFormatA4,dd.ePageOrientationPortrait)
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 2
oMyPos.X2 = 14
oMyPos.Y1 = 2
oMyPos.Y2 = 14
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling.ScaledOutput
oMy2DAxisSystem.Settings.AxisScaleMode = dd.e2DAxisScalingModeRangeOfValues
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AxisScaleMode_IRepD2AxisSettingsInt.htm`*
