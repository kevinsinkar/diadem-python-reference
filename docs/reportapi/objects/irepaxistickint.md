---
title: "IRepAxisTickInt"
description: "The AxisTickObject object provides the tick properties of a 3D axis system or a polar axis system in DIAdem REPORT."
---

# IRepAxisTickInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AxisTickObject

The AxisTickObject object provides the tick properties of a 3D axis system or a polar axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "My3DAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMyAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyXScaling = oMyAxisSystem.AxisList.X.Scaling
oMyXScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyXScaling.Tick.SpacingType = dd.eAxisTickSpacingDefinedByDistance
oMyXScaling.Tick.Distance = 0.5
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepaxistickint-channel/">Channel</a> | <a href="../../properties/irepaxistickint-distance/">Distance</a> | <a href="../../properties/irepaxistickint-spacingtype/">SpacingType</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3axisxscalingint/">3DAxisXScaling</a>.<a href="../../properties/irepd3axisxscalingint-tick/">Tick</a> | <a href="../irepd3axisyscalingint/">3DAxisYScaling</a>.<a href="../../properties/irepd3axisyscalingint-tick/">Tick</a> | <a href="../irepd3axiszscalingint/">3DAxisZScaling</a>.<a href="../../properties/irepd3axiszscalingint-tick/">Tick</a> | <a href="../ireppolaraxisscalingint/">PolarAxisScaling</a>.<a href="../../properties/ireppolaraxisscalingint-tick/">Tick</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepAxisTickInt.htm`*
