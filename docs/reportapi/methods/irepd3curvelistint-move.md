---
title: "IRepD3CurveListInt.Move"
description: "Moves in a 3D axis system in DIAdem REPORT a curve to a different position."
---

# IRepD3CurveListInt.Move

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Move for 3DCurves

Moves in a 3D axis system in DIAdem REPORT a curve to a different position.

## Signature

```python
obj.Move(NameOrIndexFrom, NameOrIndexTo)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPosition = oMy3DAxisSys.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 10
oMyPosition.Y2 = 40
oMyCurve1 = oMy3DAxisSys.Curves3D.Add(dd.e3DShapeLine, "MyNewCurve1")
oMyCurve1.Shape.XChannel.Reference= "[2]/[1]"
oMyCurve1.Shape.YChannel.Reference = "[2]/[2]"
oMyCurve1.Shape.ZChannel.Reference = "[2]/[3]"
oMyCurve2 = oMy3DAxisSys.Curves3D.Add(dd.e3DShapeLine, "MyNewCurve2")
oMyCurve2.Shape.XChannel.Reference= "[3]/[1]"
oMyCurve2.Shape.YChannel.Reference = "[3]/[2]"
oMyCurve2.Shape.ZChannel.Reference = "[3]/[3]"
oMy3DCurves = oMy3DAxisSys.Curves3D
oMy3DCurves.Move(1,2)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Move_IRepD3CurveListInt.htm`*
