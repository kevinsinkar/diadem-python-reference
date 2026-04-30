---
title: "IRepPieChartSettingsInt.DisplayMode"
description: "Specifies whether DIAdem displays the pie chart as a pie or as a doughnut. In the ring display you specify the size of the hole with the property HoleSize ."
---

# IRepPieChartSettingsInt.DisplayMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DisplayMode for PieChartSettings

Specifies whether DIAdem displays the pie chart as a pie or as a doughnut. In the ring display you specify the size of the hole with the property HoleSize .

## Signature

```python
obj.DisplayMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePieChartDisplayModePie` | 0 | Pie |
| `ePieChartDisplayModeDoughnut` | 1 | Doughnut |

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
oMySettings = oMyPieChart.Settings
oMySettings.DisplayMode = dd.ePieChartDisplayModeDoughnut
oMySettings.HoleSize = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DisplayMode_IRepPieChartSettingsInt.htm`*
