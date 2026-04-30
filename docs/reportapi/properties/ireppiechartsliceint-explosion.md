---
title: "IRepPieChartSliceInt.Explosion"
description: "Specifies the displacement of a segment in a pie chart in DIAdem REPORT. Use the property Explosion for PieChartSettings to shift all segments."
---

# IRepPieChartSliceInt.Explosion

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Explosion for PieChartSlice

Specifies the displacement of a segment in a pie chart in DIAdem REPORT. Use the property Explosion for PieChartSettings to shift all segments.

## Signature

```python
obj.Explosion
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

*Source: `ReportApi/properties/Report_property_Explosion_IRepPieChartSliceInt.htm`*
