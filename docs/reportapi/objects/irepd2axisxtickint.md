---
title: "IRepD2AxisXTickInt"
description: "The 2DAxisXTick object provides the tick properties of an x-axis scaling in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXTickInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisXTick

The 2DAxisXTick object provides the tick properties of an x-axis scaling in a 2D axis system in DIAdem REPORT.

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
<p><a href="../../properties/irepd2axisxtickint-channel/">Channel</a> | <a href="../../properties/irepd2axisxtickint-distance/">Distance</a> | <a href="../../properties/irepd2axisxtickint-origin/">Origin</a> | <a href="../../properties/irepd2axisxtickint-spacingtype/">SpacingType</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisxscalingint/">2DAxisXScaling</a>.<a href="../../properties/irepd2axisxscalingint-tick/">Tick</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisXTickInt.htm`*
