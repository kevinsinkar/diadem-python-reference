---
title: "IRepD2CurveListInt.Add"
description: "Generates a new curve in a 2D axis system in DIAdem REPORT."
---

# IRepD2CurveListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for 2DCurves

Generates a new curve in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Add(ShapeType, Name)
```

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepD2CurveListInt.htm`*
