---
title: "IRepPieChartSelectedSubObjectsListInt.AddPieChart"
description: "Selects the subobject of a pie chart associated with a specific index in DIAdem REPORT."
---

# IRepPieChartSelectedSubObjectsListInt.AddPieChart

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: AddPieChart for PieChartSelectedElements

Selects the subobject of a pie chart associated with a specific index in DIAdem REPORT.

## Signature

```python
return_value = obj.AddPieChart(ElementType, Index)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePieChartElementMain` | 0 | Main object |
| `ePieChartElementSlice` | 1 | Segment |
| `ePieChartElementLabel` | 2 | Segment label |
| `ePieChartElementLegend` | 3 | Legend |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMyPieChart = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPieChart, "MyPieChart")
oMyPos = oMyPieChart.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurvePieChart = oMyPieChart.CurvePieChart # CurvePieChartPieChart
oMyCurvePieChart.Channel.Reference = "[5]/[4]"
dd.Report.Refresh()
oMyPieChart.SelectedElements.AddPieChart(dd.ePieChartElementSlice, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_AddPieChart_IRepPieChartSelectedSubObjectsListInt.htm`*
