---
title: "IRepPieChartSettingsInt.InclinationAngle"
description: "Specifies the inclination angle of a pie chart in DIAdem REPORT."
---

# IRepPieChartSettingsInt.InclinationAngle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: InclinationAngle for PieChartSettings

Specifies the inclination angle of a pie chart in DIAdem REPORT.

## Signature

```python
obj.InclinationAngle
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
oMyCurve = oMyPieChart.CurvePieChart
oMyCurve.Channel.Reference = "[5]/[4]"
oMySettings = oMyPieChart.Settings
oMySettings.InclinationAngle = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_InclinationAngle_IRepPieChartSettingsInt.htm`*
