---
title: "IRepD2YAxisScaledOutputSettingsInt.AutoScalingType"
description: "Specifies whether and how DIAdem REPORT specifies the origin, the begin, and the tick interval for scaled display of the y-axis."
---

# IRepD2YAxisScaledOutputSettingsInt.AutoScalingType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AutoScalingType for 2DYAxisScaledOutput

Specifies whether and how DIAdem REPORT specifies the origin, the begin, and the tick interval for scaled display of the y-axis.

## Signature

```python
obj.AutoScalingType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisAutoScalingScaledOutputManual` | 0 | Manual |
| `eAxisAutoScalingScaledOutputBeginOriginTickAutomatic` | 1 | Begin and tick distance automatic |
| `eAxisAutoScalingScaledOutputCompleteAutomatic` | 2 | Fully automatic |
| `eAxisAutoScalingScaledOutputCustom` | 3 | User-defined scaling |

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

*Source: `ReportApi/properties/Report_property_AutoScalingType_IRepD2YAxisScaledOutputSettingsInt.htm`*
