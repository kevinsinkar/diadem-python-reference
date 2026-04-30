---
title: "IRepD2AxisXTickInt.Distance"
description: "Specifies in a 2D axis system in DIAdem REPORT the interval between the ticks you want labeled on the x-axis, in units of the axis range. If the scaling is not "
---

# IRepD2AxisXTickInt.Distance

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Distance for 2DAxisXTick

Specifies in a 2D axis system in DIAdem REPORT the interval between the ticks you want labeled on the x-axis, in units of the axis range. If the scaling is not logarithmic, the value of the Distance property is the space between the main ticks you want to label. If the scaling is logarithmic, DIAdem interprets the values before the decimal point and the values after the decimal point of the Distance property separately. The integer value before the decimal point specifies the steps between two labels, which are powers of ten. For example, if the axis origin and the tick interval have the value 1, DIAdem labels the ticks at 10 0 , 10 1 , 10 2 and so on. For example, if you assign the value 3 to the tick interval, DIAdem labels the ticks at 10 0 , 10 3 , 10 6 and so on. The reciprocal value after the decimal point, specifies intervals that you want to label in the ranges defined by the value before the decimal point. For example, if you assign the value 1.25 to the Distance property, DIAdem divides the area into quarters.

## Signature

```python
obj.Distance
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
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyXScaling.Type = dd.e2DXScalingLogarithmic
oMyXScaling.Begin = 0.01
oMyXScaling.End = 100
oMyXScaling.Origin = 1
oMyXScaling.Tick.Distance = 1
oMyXScaling.MiniTickCount = 10
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyYScaling.Type = dd.e2DYScalingLinear
oMyYScaling.Begin = 0
oMyYScaling.End = 100
oMyYScaling.Origin = 50
oMyYScaling.Tick.Distance = 12.5
oMyYScaling.MiniTickCount = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Distance_IRepD2AxisXTickInt.htm`*
