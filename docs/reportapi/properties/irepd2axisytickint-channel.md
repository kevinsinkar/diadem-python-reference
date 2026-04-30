---
title: "IRepD2AxisYTickInt.Channel"
description: "Specifies the tick channel for the y-axis scaling of a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYTickInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for 2DAxisYTick

Specifies the tick channel for the y-axis scaling of a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Channel
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
oMyXScaling.Tick.SpacingType = dd.eAxisTickSpacingReadFromChannel
oMyXScaling.Tick.Channel.Reference = "[1]/[2]"
oMyXScaling.MiniTickCount = 10
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyYScaling.Type = dd.e2DYScalingLinear
oMyYScaling.Begin = 0
oMyYScaling.End = 100
oMyYScaling.Origin = 50
oMyYScaling.Tick.SpacingType = dd.eAxisTickSpacingReadFromChannel
oMyYScaling.Tick.Channel.Reference = "[1]/[2]"
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

*Source: `ReportApi/properties/Report_property_Channel_IRepD2AxisYTickInt.htm`*
