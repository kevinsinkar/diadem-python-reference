---
title: "IRepD2CurveListInt.Copy"
description: "Copies a curve in a 2D axis system in DIAdem REPORT and adds this curve to the axis system."
---

# IRepD2CurveListInt.Copy

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Copy for 2DCurves

Copies a curve in a 2D axis system in DIAdem REPORT and adds this curve to the axis system.

## Signature

```python
return_value = obj.Copy(NameOrIndex, NewName, InsertBeforeNameOrIndex)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSys.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyCurve1 = oMy2DAxisSys.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve1")
oMyCurve1.Shape.XChannel.Reference= "[1]/[1]"
oMyCurve1.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurves = oMy2DAxisSys.Curves2D
oMyCurve2 = oMy2DCurves.Copy("MyNewCurve1","NewCurve2",1)
print("Number of curves: " + oMy2DCurves.Count)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Copy_IRepD2CurveListInt.htm`*
