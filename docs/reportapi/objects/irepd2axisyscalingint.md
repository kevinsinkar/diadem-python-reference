---
title: "IRepD2AxisYScalingInt"
description: "The 2DAxisYScaling object provides the scaling properties for a y-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYScalingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisYScaling

The 2DAxisYScaling object provides the scaling properties for a y-axis in a 2D axis system in DIAdem REPORT.

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
<p><a href="../../properties/irepd2axisyscalingint-autoscalingtype/">AutoScalingType</a> | <a href="../../properties/irepd2axisyscalingint-begin/">Begin</a> | <a href="../../properties/irepd2axisyscalingint-customscalingid/">CustomScalingID</a> | <a href="../../properties/irepd2axisyscalingint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/irepd2axisyscalingint-end/">End</a> | <a href="../../properties/irepd2axisyscalingint-minitickcount/">MiniTickCount</a> | <a href="../../properties/irepd2axisyscalingint-origin/">Origin</a> | <a href="../../properties/irepd2axisyscalingint-scaledoutput/">ScaledOutput</a> | <a href="../../properties/irepd2axisyscalingint-spanwidth/">SpanWidth</a> | <a href="../../properties/irepd2axisyscalingint-synchronizationid/">SynchronizationID</a> | <a href="../../properties/irepd2axisyscalingint-tick/">Tick</a> | <a href="../../properties/irepd2axisyscalingint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisyint/">2DAxisY</a>.<a href="../../properties/irepd2axisyint-scaling/">Scaling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisYScalingInt.htm`*
