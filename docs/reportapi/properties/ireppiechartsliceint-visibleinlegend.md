---
title: "IRepPieChartSliceInt.VisibleInLegend"
description: "Specifies whether DIAdem REPORT displays the legend of a segment in a pie chart."
---

# IRepPieChartSliceInt.VisibleInLegend

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: VisibleInLegend for PieChartSlice

Specifies whether DIAdem REPORT displays the legend of a segment in a pie chart.

## Signature

```python
obj.VisibleInLegend
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
oMyPieChart.CurvePieChart.Slices(2).VisibleInLegend = False
oMySliceLabel = oMyCurvePieChart.SliceLabel
oMySliceLabel.CategoryVisible = True
oMySliceLabel.Channel.Reference = "[5]/[1]"
oMySliceLabel.CategoryMode = dd.eCategoryModeChannel
oMyLegend = oMyPieChart.Legend
oMyLegend.Visible = True
oMyCurveLegendPos = oMyLegend.Position
oMyCurveLegendPos.RelativePosition = dd.eLegendRelativePositionTopLeft
oMyCurveLegendPos.SizeMode = dd.eLegendSizeElementwise
oMyCurveLegendPos.ElementHeight = 5
oMyCurveLegendPos.ElementWidth = 35
oMyLegend.Settings.Font.Size = 4
oMyLegendColumns = oMyLegend.Columns
oMyLegendColumns(1).Title = "First title"
oMyLegendColumns(1).Type = dd.eLegendTextPieChartCustomText
oMyLegendColumns(1).RelativeWidth = 2
oMyLegendColumns(1).Text = "First col - longer text"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_VisibleInLegend_IRepPieChartSliceInt.htm`*
