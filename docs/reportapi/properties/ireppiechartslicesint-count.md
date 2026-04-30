---
title: "IRepPieChartSlicesInt.Count"
description: "Specifies the number of prepared segments in a pie chart in DIAdem REPORT. DIAdem saves the number of prepared segments in the layout. This way you can paramete"
---

# IRepPieChartSlicesInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for PieChartSlices

Specifies the number of prepared segments in a pie chart in DIAdem REPORT. DIAdem saves the number of prepared segments in the layout. This way you can parameterize segments without having to load a channel. DIAdem displays as many segments in the layout as the length of the loaded data is. If the value of the property is smaller than the loaded data channel, DIAdem increases the value to the length of the data channel.

## Signature

```python
obj.Count
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
oMyCurvePieChart.Slices.Count = 10
oMyPieChart.ShowPropertiesDlg()
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepPieChartSlicesInt.htm`*
