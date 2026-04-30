---
title: "IRepD3AxisZScalingInt"
description: "The 3DAxisZScaling object provides the scaling properties of the z-axis in a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisZScalingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAxisZScaling

The 3DAxisZScaling object provides the scaling properties of the z-axis in a 3D axis system in DIAdem REPORT.

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
<p><a href="../../properties/irepd3axiszscalingint-autoscalingtype/">AutoScalingType</a> | <a href="../../properties/irepd3axiszscalingint-begin/">Begin</a> | <a href="../../properties/irepd3axiszscalingint-customscalingid/">CustomScalingID</a> | <a href="../../properties/irepd3axiszscalingint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/irepd3axiszscalingint-end/">End</a> | <a href="../../properties/irepd3axiszscalingint-minitickcount/">MiniTickCount</a> | <a href="../../properties/irepd3axiszscalingint-origin/">Origin</a> | <a href="../../properties/irepd3axiszscalingint-tick/">Tick</a> | <a href="../../properties/irepd3axiszscalingint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3axiszint/">3DAxisZ</a>.<a href="../../properties/irepd3axiszint-scaling/">Scaling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3AxisZScalingInt.htm`*
