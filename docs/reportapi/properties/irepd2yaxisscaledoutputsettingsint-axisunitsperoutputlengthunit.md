---
title: "IRepD2YAxisScaledOutputSettingsInt.AxisUnitsPerOutputLengthUnit"
description: "Specifies the number of y-scaling ticks per centimeter for scaled display in a 2D axis system in DIAdem REPORT."
---

# IRepD2YAxisScaledOutputSettingsInt.AxisUnitsPerOutputLengthUnit

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AxisUnitsPerOutputLengthUnit for 2DYAxisScaledOutput

Specifies the number of y-scaling ticks per centimeter for scaled display in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.AxisUnitsPerOutputLengthUnit
```

## Python example

```python
dd.Report.NewLayout()
dd.Report.Settings.Page.Dimensions.UseScaledOutput = True
dd.Report.Settings.Page.Dimensions.ScaledHeight = 26
dd.Report.Settings.Page.Dimensions.ScaledWidth = 18
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 2
oMyPos.X2 = 14
oMyPos.Y1 = 2
oMyPos.Y2 = 20
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling.ScaledOutput
oMy2DAxisSystem.Settings.AxisScaleMode = dd.e2DAxisScalingModeForScaledOutput
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingScaledOutputBeginOriginTickAutomatic
oMyXScaling.AxisUnitsPerOutputLengthUnit = 5
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling.ScaledOutput
oMy2DAxisSystem.Settings.AxisScaleMode = dd.e2DAxisScalingModeForScaledOutput
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingScaledOutputBeginOriginTickAutomatic
oMyYScaling.AxisUnitsPerOutputLengthUnit = 3
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AxisUnitsPerOutputLengthUnit_IRepD2YAxisScaledOutputSettingsInt.htm`*
