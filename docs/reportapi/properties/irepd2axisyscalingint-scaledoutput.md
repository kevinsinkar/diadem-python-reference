---
title: "IRepD2AxisYScalingInt.ScaledOutput"
description: "Specifies the scaling properties of the x-axis in a 2D axis system in scaled display in DIAdem REPORT. To enable the scaled display, use the UseScaledOutput pro"
---

# IRepD2AxisYScalingInt.ScaledOutput

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ScaledOutput for 2DAxisYScaling

Specifies the scaling properties of the x-axis in a 2D axis system in scaled display in DIAdem REPORT. To enable the scaled display, use the UseScaledOutput property.

## Signature

```python
return_value = obj.ScaledOutput
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByBorder
oMyPos.Left = 20
oMyPos.Bottom = 20
oMyPos.Right = 20
oMyPos.Top = 20
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling.ScaledOutput
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingScaledOutputCompleteAutomatic
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling.ScaledOutput
oMyYScaling.AutoScalingType =dd.eAxisAutoScalingScaledOutputCompleteAutomatic
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ScaledOutput_IRepD2AxisYScalingInt.htm`*
