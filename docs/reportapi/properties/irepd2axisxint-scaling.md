---
title: "IRepD2AxisXInt.Scaling"
description: "Specifies the scaling of the x-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXInt.Scaling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Scaling for 2DAxisX

Specifies the scaling of the x-axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Scaling
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.XAxis.Scaling.AutoScalingType = dd.eAxisAutoScalingBeginEndManual
oMy2DAxisSystem.XAxis.Scaling.Begin = 10
oMy2DAxisSystem.XAxis.Scaling.End = 40
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Scaling_IRepD2AxisXInt.htm`*
