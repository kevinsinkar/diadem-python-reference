---
title: "IRepPolarInt.UpdateScaling"
description: "Refreshes the values which DIAdem REPORT uses to automatically scale a polar axis system. You can use the values specified automatically, for example, for manua"
---

# IRepPolarInt.UpdateScaling

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: UpdateScaling for PolarSystem

Refreshes the values which DIAdem REPORT uses to automatically scale a polar axis system. You can use the values specified automatically, for example, for manual scaling.

## Signature

```python
obj.UpdateScaling()
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyScaling = oMyPolarAxisSystem.RadialAxis.Scaling
oMyPolarAxisSystem.UpdateScaling()
oMyScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyScaling.End = int(oMyScaling.End) + 1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_UpdateScaling_IRepPolarInt.htm`*
