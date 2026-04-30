---
title: "IRepCurvelegendContentColumnsListInt.Item"
description: "Returns the column of a curve legend associated with a specific index in DIAdem REPORT."
---

# IRepCurvelegendContentColumnsListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for CurveLegendColumns

Returns the column of a curve legend associated with a specific index in DIAdem REPORT.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DaxisSystem.CurveLegend.Visible = True
oMyLegendColumns = oMy2DaxisSystem.CurveLegend.Columns
oMyLegendColumns.Add()
oMyLegendColumns(1).Type = dd.eLegendTextComment
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepCurvelegendContentColumnsListInt.htm`*
