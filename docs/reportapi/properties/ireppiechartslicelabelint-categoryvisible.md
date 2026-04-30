---
title: "IRepPieChartSliceLabelInt.CategoryVisible"
description: "Specifies whether DIAdem REPORT displays the slice labels in a pie chart."
---

# IRepPieChartSliceLabelInt.CategoryVisible

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CategoryVisible for PieChartSliceLabel

Specifies whether DIAdem REPORT displays the slice labels in a pie chart.

## Signature

```python
obj.CategoryVisible
```

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
oMyCurvePieChart = oMyPieChart.CurvePieChart
oMyCurvePieChart.Channel.Reference = "[5]/[4]"
oMyCurvePieChart.SliceLabel.CategoryVisible = False
oMySettings = oMyPieChart.Settings
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2> </h2>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CategoryVisible_IRepPieChartSliceLabelInt.htm`*
