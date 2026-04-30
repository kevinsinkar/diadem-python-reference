---
title: "IRepD3AxisZScalingInt.End"
description: "Specifies the value up to which DIAdem REPORT displays the z-axis of a 3D axis system. DIAdem REPORT only includes the End property if you assign the value eAxi"
---

# IRepD3AxisZScalingInt.End

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: End for 3DAxisZScaling

Specifies the value up to which DIAdem REPORT displays the z-axis of a 3D axis system. DIAdem REPORT only includes the End property if you assign the value eAxisScalingSimpleManual to the AutoScalingType property.

## Signature

```python
obj.End
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_End_IRepD3AxisZScalingInt.htm`*
