---
title: "IRepD2CurveListInt.Move"
description: "Moves in a 2D axis system in DIAdem REPORT a curve to a different position."
---

# IRepD2CurveListInt.Move

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Move for 2DCurves

Moves in a 2D axis system in DIAdem REPORT a curve to a different position.

## Signature

```python
obj.Move(NameOrIndexFrom, NameOrIndexTo)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSys.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 10
oMyPosition.Y2 = 40
oMyCurve1 = oMy2DAxisSys.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve1")
oMyCurve1.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve1.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve2 = oMy2DAxisSys.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve2")
oMyCurve2.Shape.XChannel.Reference= "[5]/[3]"
oMyCurve2.Shape.YChannel.Reference = "[5]/[4]"
oMy2DCurves = oMy2DAxisSys.Curves2D
oMy2DCurves.Move(1,2)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Move_IRepD2CurveListInt.htm`*
