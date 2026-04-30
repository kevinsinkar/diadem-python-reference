---
title: "IRepD3AxisYScalingInt.Tick"
description: "Specifies the properties of the y-axis ticks in a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisYScalingInt.Tick

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Tick for 3DAxisYScaling

Specifies the properties of the y-axis ticks in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Tick
```

## Python example

```python
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyXScaling = oMy3DAxisSystem.AxisList.X.Scaling
oMyXScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyXScaling.Begin = 0.1
oMyXScaling.End = 1
oMyXScaling.MiniTickCount = 4
oMyXScaling.Tick.Distance = 0.5
oMyYScaling = oMy3DAxisSystem.AxisList.Y.Scaling
oMyYScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyYScaling.Begin = 0.1
oMyYScaling.End = 0.9
oMyYScaling.MiniTickCount = 1
oMyYScaling.Tick.Distance = 0.2
oMyZScaling = oMy3DAxisSystem.AxisList.Z.Scaling
oMyZScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyZScaling.Begin = 0
oMyZScaling.End = 1
oMyZScaling.MiniTickCount = 9
oMyZScaling.Tick.Distance = 0.1
oMyZScaling.Origin = 0
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Tick_IRepD3AxisYScalingInt.htm`*
