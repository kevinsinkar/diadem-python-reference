---
title: "IRepCurvelegendContentColumnsListInt.Count"
description: "Changes the number of columns of a curve legend in DIAdem REPORT, or returns this value."
---

# IRepCurvelegendContentColumnsListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for CurveLegendColumns

Changes the number of columns of a curve legend in DIAdem REPORT, or returns this value.

## Signature

```python
obj.Count
```

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DaxisSystem.CurveLegend.Visible = True
oMyLegendColumns = oMy2DaxisSystem.CurveLegend.Columns
oMyLegendColumns.Add()
oMyLegendColumns(1).Type = dd.eLegendTextComment
dd.MsgBoxDisp(oMyLegendColumns.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepCurvelegendContentColumnsListInt.htm`*
