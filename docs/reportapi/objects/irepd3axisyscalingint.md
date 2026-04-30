---
title: "IRepD3AxisYScalingInt"
description: "The 3DAxisYScaling object provides the scaling properties of the y-axis in a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisYScalingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAxisYScaling

The 3DAxisYScaling object provides the scaling properties of the y-axis in a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMyXScaling = oMy3DAxisSystem.AxisList.X.Scaling
oMyXScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyXScaling.Begin = 0.1
oMyXScaling.End = 0.9
oMyXScaling.MiniTickCount = 10
oMyXScaling.Tick.Distance = 0.2
oMyYScaling = oMy3DAxisSystem.AxisList.Y.Scaling
oMyYScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyYScaling.Begin = 0.1
oMyYScaling.End = 0.9
oMyYScaling.MiniTickCount = 10
oMyYScaling.Tick.Distance = 0.2
oMyZScaling = oMy3DAxisSystem.AxisList.Z.Scaling
oMyZScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyZScaling.Begin = 0.3
oMyZScaling.End = -0.9
oMyZScaling.MiniTickCount = 10
oMyZScaling.Tick.Distance = 0.2
oMyZScaling.Origin = 0
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3axisyscalingint-autoscalingtype/">AutoScalingType</a> | <a href="../../properties/irepd3axisyscalingint-begin/">Begin</a> | <a href="../../properties/irepd3axisyscalingint-customscalingid/">CustomScalingID</a> | <a href="../../properties/irepd3axisyscalingint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/irepd3axisyscalingint-end/">End</a> | <a href="../../properties/irepd3axisyscalingint-minitickcount/">MiniTickCount</a> | <a href="../../properties/irepd3axisyscalingint-origin/">Origin</a> | <a href="../../properties/irepd3axisyscalingint-tick/">Tick</a> | <a href="../../properties/irepd3axisyscalingint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3axisyint/">3DAxisY</a>.<a href="../../properties/irepd3axisyint-scaling/">Scaling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3AxisYScalingInt.htm`*
