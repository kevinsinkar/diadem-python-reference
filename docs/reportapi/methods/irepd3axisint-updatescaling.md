---
title: "IRepD3AxisInt.UpdateScaling"
description: "Refreshes the values which DIAdem REPORT uses to automatically scale a 3D axis system. You can use the values specified automatically, for example, for manual s"
---

# IRepD3AxisInt.UpdateScaling

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: UpdateScaling for 3DAxisSystem

Refreshes the values which DIAdem REPORT uses to automatically scale a 3D axis system. You can use the values specified automatically, for example, for manual scaling.

## Signature

```python
obj.UpdateScaling()
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyZScaling = oMy3DAxisSystem.AxisList.Z.Scaling
oMy3DAxisSystem.UpdateScaling()
oMyZScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyZScaling.End = int(oMyZScaling.End) + 1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_UpdateScaling_IRepD3AxisInt.htm`*
