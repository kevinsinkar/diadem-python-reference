---
title: "IRepPieChartSliceLabelInt.CategoryMode"
description: "Specifies in a pie chart in DIAdem REPORT whether DIAdem extracts the segment labels from a channel or whether you specify the segment labels manually."
---

# IRepPieChartSliceLabelInt.CategoryMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CategoryMode for PieChartSliceLabel

Specifies in a pie chart in DIAdem REPORT whether DIAdem extracts the segment labels from a channel or whether you specify the segment labels manually.

## Signature

```python
obj.CategoryMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCategoryModeChannel` | 0 | Channel |
| `eCategoryModeFreeText` | 1 | Free text |

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
oMyCurvePieChart.SliceLabel.Channel.Reference = "[5]/[1]"
oMyCurvePieChart.SliceLabel.CategoryMode = dd.eCategoryModeChannel
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CategoryMode_IRepPieChartSliceLabelInt.htm`*
