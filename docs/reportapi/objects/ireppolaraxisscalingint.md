---
title: "IRepPolarAxisScalingInt"
description: "The PolarAxisScaling object provides the radial axis scaling for a polar axis system in DIAdem REPORT."
---

# IRepPolarAxisScalingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarAxisScaling

The PolarAxisScaling object provides the radial axis scaling for a polar axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarAxisSystem.RadialAxis.Scaling.Type = dd.ePolarScalingLinear
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolaraxisscalingint-autoscalingtype/">AutoScalingType</a> | <a href="../../properties/ireppolaraxisscalingint-begin/">Begin</a> | <a href="../../properties/ireppolaraxisscalingint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/ireppolaraxisscalingint-end/">End</a> | <a href="../../properties/ireppolaraxisscalingint-minitickcount/">MiniTickCount</a> | <a href="../../properties/ireppolaraxisscalingint-origin/">Origin</a> | <a href="../../properties/ireppolaraxisscalingint-tick/">Tick</a> | <a href="../../properties/ireppolaraxisscalingint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarradialaxisint/">PolarRadialAxis</a>.<a href="../../properties/ireppolarradialaxisint-scaling/">Scaling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarAxisScalingInt.htm`*
