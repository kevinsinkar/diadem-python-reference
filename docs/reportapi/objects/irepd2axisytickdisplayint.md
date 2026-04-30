---
title: "IRepD2AxisYTickDisplayInt"
description: "The 2DAxisYTickDisplay object provides the axis tick properties in a y-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYTickDisplayInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisYTickDisplay

The 2DAxisYTickDisplay object provides the axis tick properties in a y-axis in a 2D axis system in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisytickdisplayint-size/">Size</a> | <a href="../../properties/irepd2axisytickdisplayint-type/">Type</a> | <a href="../../properties/irepd2axisytickdisplayint-useautosize/">UseAutoSize</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisyint/">2DAxisY</a>.<a href="../../properties/irepd2axisyint-tickdisplay/">TickDisplay</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisYTickDisplayInt.htm`*
