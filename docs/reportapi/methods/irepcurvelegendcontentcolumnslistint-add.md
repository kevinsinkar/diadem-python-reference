---
title: "IRepCurvelegendContentColumnsListInt.Add"
description: "Adds a column to the curve legend of a 2D axis system in DIAdem REPORT."
---

# IRepCurvelegendContentColumnsListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for CurveLegendColumns

Adds a column to the curve legend of a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Add()
```

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DaxisSystem.CurveLegend.Visible = True
oMyLegendColumn = oMy2DaxisSystem.CurveLegend.Columns.Add()
oMyLegendColumn.Type = dd.eLegendTextComment
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepCurvelegendContentColumnsListInt.htm`*
