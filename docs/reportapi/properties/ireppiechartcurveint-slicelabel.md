---
title: "IRepPieChartCurveInt.SliceLabel"
description: "Specifies the segment labels in a pie chart in DIAdem REPORT."
---

# IRepPieChartCurveInt.SliceLabel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SliceLabel for PieChartCurve

Specifies the segment labels in a pie chart in DIAdem REPORT.

## Signature

```python
return_value = obj.SliceLabel
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
oMyCurvePieChart = oMyPieChart.CurvePieChart # CurvePieChartPieChart
oMyCurvePieChart.Channel.Reference = "[5]/[4]"
oMySliceLabel = oMyCurvePieChart.SliceLabel
oMySliceLabel.PhysicalValueVisible = True
oMySliceLabel.PhysicalValueFormat = "d.dd"
oMySliceLabel.RelativeValueVisible = True
oMySliceLabel.RelativeValueFormat = "d.dd"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SliceLabel_IRepPieChartCurveInt.htm`*
