---
title: "IRepPolarCurveListInt.Move"
description: "Moves in a polar axis system in DIAdem REPORT a polar curve to a different position."
---

# IRepPolarCurveListInt.Move

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Move for PolarCurves

Moves in a polar axis system in DIAdem REPORT a polar curve to a different position.

## Signature

```python
obj.Move(NameOrIndexFrom, NameOrIndexTo)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSys.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 10
oMyPosition.Y2 = 40
oMyCurve1 = oMyPolarAxisSys.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve1")
oMyCurve1.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve1.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve2 = oMyPolarAxisSys.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve2")
oMyCurve2.Shape.XChannel.Reference= "[5]/[3]"
oMyCurve2.Shape.YChannel.Reference = "[5]/[4]"
oMyPolarCurves = oMyPolarAxisSys.CurvesPolar
oMyPolarCurves.Move(1,2)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Move_IRepPolarCurveListInt.htm`*
