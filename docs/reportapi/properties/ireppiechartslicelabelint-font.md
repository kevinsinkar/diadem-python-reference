---
title: "IRepPieChartSliceLabelInt.Font"
description: "Specifies the font for a scale label in a pie chart in DIAdem REPORT."
---

# IRepPieChartSliceLabelInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for PieChartSliceLabel

Specifies the font for a scale label in a pie chart in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
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
oMyLabel = oMyCurvePieChart.SliceLabel
oMyLabel.Channel.Reference = "[5]/[1]"
oMyLabel.Font.Size = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepPieChartSliceLabelInt.htm`*
