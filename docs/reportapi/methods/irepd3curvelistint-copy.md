---
title: "IRepD3CurveListInt.Copy"
description: "Copies a curve in a 3D axis system in DIAdem REPORT and adds this curve to the axis system."
---

# IRepD3CurveListInt.Copy

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Copy for 3DCurves

Copies a curve in a 3D axis system in DIAdem REPORT and adds this curve to the axis system.

## Signature

```python
return_value = obj.Copy(NameOrIndex, NewName, InsertBeforeNameOrIndex)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPosition = oMy3DAxisSys.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyCurve1 = oMy3DAxisSys.Curves3D.Add(dd.e3DShapeLine, "MyNewCurve1")
oMyCurve1.Shape.XChannel.Reference= "[3]/[1]"
oMyCurve1.Shape.YChannel.Reference = "[3]/[2]"
oMyCurve1.Shape.ZChannel.Reference = "[3]/[3]"
oMy3DCurves = oMy3DAxisSys.Curves3D
oMyCurve2 = oMy3DCurves.Copy("MyNewCurve1","NewCurve2",1)
print("Number of curves: " + oMy3DCurves.Count)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Copy_IRepD3CurveListInt.htm`*
