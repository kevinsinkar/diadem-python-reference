---
title: "IRepCurveLegendInt.Columns"
description: "Specifies all columns in the curve legend of an axis system in DIAdem REPORT, except the standard column."
---

# IRepCurveLegendInt.Columns

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Columns for CurveLegend

Specifies all columns in the curve legend of an axis system in DIAdem REPORT, except the standard column.

## Signature

```python
return_value = obj.Columns
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyCurveLegend = oMy2DAxisSystem.CurveLegend
oMyCurveLegend.Visible = True
dd.MsgBoxDisp(oMyCurveLegend.Columns.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Columns_IRepCurveLegendInt.htm`*
