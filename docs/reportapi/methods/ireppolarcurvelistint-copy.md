---
title: "IRepPolarCurveListInt.Copy"
description: "Copies a curve in a polar axis system in DIAdem REPORT and adds it to the polar axis system."
---

# IRepPolarCurveListInt.Copy

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Copy for PolarCurves

Copies a curve in a polar axis system in DIAdem REPORT and adds it to the polar axis system.

## Signature

```python
return_value = obj.Copy(NameOrIndex, NewName, InsertBeforeNameOrIndex)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyCurves = oMyPolarAxisSys.CurvesPolar
oMyCurve = oMyCurves.Add(dd.ePolarShapeLine, "MyNewCurve1")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve2 = oMyCurves.Copy("MyNewCurve1","NewCurve2",1)
print("Number of curves: " + oMyCurves.Count)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Copy_IRepPolarCurveListInt.htm`*
