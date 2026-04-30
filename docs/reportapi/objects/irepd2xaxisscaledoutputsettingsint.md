---
title: "IRepD2XAxisScaledOutputSettingsInt"
description: "The 2DXAxisScaledOutput object provides the scaling properties of the x-axis in a 2D axis system in scaled display in DIAdem REPORT. To enable the scaled displa"
---

# IRepD2XAxisScaledOutputSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DXAxisScaledOutput

The 2DXAxisScaledOutput object provides the scaling properties of the x-axis in a 2D axis system in scaled display in DIAdem REPORT. To enable the scaled display, use the UseScaledOutput property.

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
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2xaxisscaledoutputsettingsint-autoscalingtype/">AutoScalingType</a> | <a href="../../properties/irepd2xaxisscaledoutputsettingsint-axisunitsperoutputlengthunit/">AxisUnitsPerOutputLengthUnit</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisxscalingint/">2DAxisXScaling</a>.<a href="../../properties/irepd2axisxscalingint-scaledoutput/">ScaledOutput</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2XAxisScaledOutputSettingsInt.htm`*
