---
title: "IRepD2AxisXScalingInt.SpanWidth"
description: "Specifies the difference between the end value and the start value of the x-axis in a 2D axis system in DIAdem REPORT. Assign the value eAxisAutoScalingSpanWidt"
---

# IRepD2AxisXScalingInt.SpanWidth

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SpanWidth for 2DAxisXScaling

Specifies the difference between the end value and the start value of the x-axis in a 2D axis system in DIAdem REPORT. Assign the value eAxisAutoScalingSpanWidthTickManual to the property AutoScalingType if you want to specify the span width manually.

## Signature

```python
obj.SpanWidth
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
oMyXScaling.Type = dd.e2DXScalingLinear
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingSpanWidthTickManual
oMyXScaling.Tick.Distance = 5
oMyXScaling.MiniTickCount = 5
oMyXScaling.SpanWidth = 10
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.Type = dd.e2DYScalingLinear
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingSpanWidthTickManual
oMyYScaling.Tick.Distance = 5
oMyYScaling.MiniTickCount = 5
oMyYScaling.SpanWidth = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SpanWidth_IRepD2AxisXScalingInt.htm`*
