---
title: "IRepD2AxisXScalingInt"
description: "The 2DAxisXScaling object provides the x-axis scaling properties of a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXScalingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisXScaling

The 2DAxisXScaling object provides the x-axis scaling properties of a 2D axis system in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisxscalingint-autoscalingtype/">AutoScalingType</a> | <a href="../../properties/irepd2axisxscalingint-begin/">Begin</a> | <a href="../../properties/irepd2axisxscalingint-customscalingid/">CustomScalingID</a> | <a href="../../properties/irepd2axisxscalingint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/irepd2axisxscalingint-end/">End</a> | <a href="../../properties/irepd2axisxscalingint-minitickcount/">MiniTickCount</a> | <a href="../../properties/irepd2axisxscalingint-origin/">Origin</a> | <a href="../../properties/irepd2axisxscalingint-scaledoutput/">ScaledOutput</a> | <a href="../../properties/irepd2axisxscalingint-spanwidth/">SpanWidth</a> | <a href="../../properties/irepd2axisxscalingint-synchronizationid/">SynchronizationID</a> | <a href="../../properties/irepd2axisxscalingint-tick/">Tick</a> | <a href="../../properties/irepd2axisxscalingint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisxint/">2DAxisX</a>.<a href="../../properties/irepd2axisxint-scaling/">Scaling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisXScalingInt.htm`*
