---
title: "IRepD2CurveListInt.ChangeShape"
description: "Changes the display mode of a curve in a 2D axis system in DIAdem REPORT."
---

# IRepD2CurveListInt.ChangeShape

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ChangeShape for 2DCurves

Changes the display mode of a curve in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.ChangeShape(NameOrIndex, ShapeType)
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "MyAxisSystem")
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.Report.Refresh()
dd.Pause(5)
oMy2DAxisSystem.Curves2D.ChangeShape("MyCurve",dd.e2DShapeSpikes)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ChangeShape_IRepD2CurveListInt.htm`*
