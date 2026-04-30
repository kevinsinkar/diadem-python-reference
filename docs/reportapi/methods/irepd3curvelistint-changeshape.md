---
title: "IRepD3CurveListInt.ChangeShape"
description: "Changes the display mode of a curve in a 3D axis system in DIAdem REPORT."
---

# IRepD3CurveListInt.ChangeShape

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ChangeShape for 3DCurves

Changes the display mode of a curve in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.ChangeShape(NameOrIndex, ShapeType)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "MyAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeLine, "My3DCurve")
oMy3DCurve.Shape.XChannel.Reference = "[3]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[3]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[3]/[3]"

dd.Report.Refresh()
dd.Pause(5)
oMy3DAxisSystem.Curves3D.ChangeShape("My3DCurve",dd.e3DShapeSpikes)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ChangeShape_IRepD3CurveListInt.htm`*
