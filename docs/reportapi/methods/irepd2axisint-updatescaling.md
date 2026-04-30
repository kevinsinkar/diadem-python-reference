---
title: "IRepD2AxisInt.UpdateScaling"
description: "Refreshes the values which DIAdem REPORT uses to automatically scale a 2D axis system. You can use the values specified automatically, for example, for manual s"
---

# IRepD2AxisInt.UpdateScaling

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: UpdateScaling for 2DAxisSystem

Refreshes the values which DIAdem REPORT uses to automatically scale a 2D axis system. You can use the values specified automatically, for example, for manual scaling.

## Signature

```python
obj.UpdateScaling()
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMy2DAxisSystem.UpdateScaling()
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingBeginEndManual
oMyYScaling.End = int(oMyYScaling.End) + 1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_UpdateScaling_IRepD2AxisInt.htm`*
