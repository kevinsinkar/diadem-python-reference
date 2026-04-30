---
title: "IRepPieChartSliceInt.Enable"
description: "Specifies whether DIAdem displays a segment in a pie chart in DIAdem REPORT. If DIAdem hides a segment, the percentage values of the other segments are automati"
---

# IRepPieChartSliceInt.Enable

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Enable for PieChartSlice

Specifies whether DIAdem displays a segment in a pie chart in DIAdem REPORT. If DIAdem hides a segment, the percentage values of the other segments are automatically converted.

## Signature

```python
obj.Enable
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
oMyCurvePieChart.Slices(2).Enable = False
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Enable_IRepPieChartSliceInt.htm`*
