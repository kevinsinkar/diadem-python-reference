---
title: "IRepPieChartInt.Settings"
description: "Specifies the general settings of a pie chart in DIAdem REPORT."
---

# IRepPieChartInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for PieChart

Specifies the general settings of a pie chart in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
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
oMyPieChart.CurvePieChart.Channel.Reference = "[5]/[4]"
oMySettings = oMyPieChart.Settings
oMySettings.ShowBorder = True
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.BorderLine.Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepPieChartInt.htm`*
