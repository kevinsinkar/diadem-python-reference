---
title: "IRepD2AxisYTickDisplayInt.Type"
description: "Specifies on which side of the y-axis DIAdem REPORT plots the axis ticks in a 2D axis system."
---

# IRepD2AxisYTickDisplayInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 2DAxisYTickDisplay

Specifies on which side of the y-axis DIAdem REPORT plots the axis ticks in a 2D axis system.

## Signature

```python
obj.Type
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
oMyTickDisplay = oMy2DAxisSystem.YAxis.TickDisplay
oMyTickDisplay.Size = 2
oMyTickDisplay.Type = dd.e2DAxisYTickBothSides
oMyTickDisplay.UseAutoSize = False
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

*Source: `ReportApi/properties/Report_property_Type_IRepD2AxisYTickDisplayInt.htm`*
