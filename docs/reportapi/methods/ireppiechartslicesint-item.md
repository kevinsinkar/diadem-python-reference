---
title: "IRepPieChartSlicesInt.Item"
description: "Returns the category of a specific index of a segment in DIAdem REPORT."
---

# IRepPieChartSlicesInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for PieChartSlices

Returns the category of a specific index of a segment in DIAdem REPORT.

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
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm", "TDM", "")
dd.Report.NewLayout()
oMyPieChart = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPieChart, "MyPieChart")
oMyPos = oMyPieChart.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurvePieChart = oMyPieChart.CurvePieChart
oMyCurvePieChart.Channel.Reference = "[5]/[4]"
oMyCurvePieChart.SliceLabel.Channel.Reference = "[5]/[1]"
oMyCurvePieChart.SliceLabel.CategoryMode = dd.eCategoryModeChannel
oMyCurvePieChart.Slices.Item(2).Explosion = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepPieChartSlicesInt.htm`*
