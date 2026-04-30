---
title: "IRepPieChartSlicesInt.Remove"
description: "Deletes a prepared segment in a pie chart in DIAdem REPORT. DIAdem saves the number of prepared segments in the layout. This way you can parameterize segments w"
---

# IRepPieChartSlicesInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for PieChartSlices

Deletes a prepared segment in a pie chart in DIAdem REPORT. DIAdem saves the number of prepared segments in the layout. This way you can parameterize segments without having to load a channel. DIAdem displays as many segments in the layout as the length of the loaded data is.

## Signature

```python
obj.Remove(Index)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm", "TDM", "")
dd.Report.NewLayout()
oMyPieChart = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPieChart, "MyPieChart")
oMyCurvePieChart = oMyPieChart.CurvePieChart
oMyCurvePieChart.Slices.Count = 10
oMyCurvePieChart.Slices.Remove(3)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepPieChartSlicesInt.htm`*
