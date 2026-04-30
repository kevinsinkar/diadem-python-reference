---
title: "IRepPieChartSettingsInt"
description: "The PieChartSettings object provides general properties of a pie chart in DIAdem REPORT."
---

# IRepPieChartSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PieChartSettings

The PieChartSettings object provides general properties of a pie chart in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppiechartsettingsint-apertureangle/">ApertureAngle</a> | <a href="../../properties/ireppiechartsettingsint-displaymode/">DisplayMode</a> | <a href="../../properties/ireppiechartsettingsint-explosion/">Explosion</a> | <a href="../../properties/ireppiechartsettingsint-holesize/">HoleSize</a> | <a href="../../properties/ireppiechartsettingsint-inclinationangle/">InclinationAngle</a> | <a href="../../properties/ireppiechartsettingsint-sliceedge/">SliceEdge</a> | <a href="../../properties/ireppiechartsettingsint-startangle/">StartAngle</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppiechartint/">PieChart</a>.<a href="../../properties/ireppiechartint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPieChartSettingsInt.htm`*
