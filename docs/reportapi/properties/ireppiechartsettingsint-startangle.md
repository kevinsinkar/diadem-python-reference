---
title: "IRepPieChartSettingsInt.StartAngle"
description: "Specifies the angle of the first segment in a pie chart in DIAdem REPORT."
---

# IRepPieChartSettingsInt.StartAngle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: StartAngle for PieChartSettings

Specifies the angle of the first segment in a pie chart in DIAdem REPORT.

## Signature

```python
obj.StartAngle
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
oMySettings = oMyPieChart.Settings
oMySettings.ApertureAngle = 180
oMySettings.StartAngle = 270
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_StartAngle_IRepPieChartSettingsInt.htm`*
