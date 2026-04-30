---
title: "IRepPieChartSliceEdgeInt.Mode"
description: "Specifies whether DIAdem REPORT displays the segments in a pie chart."
---

# IRepPieChartSliceEdgeInt.Mode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Mode for PieChartSliceEdge

Specifies whether DIAdem REPORT displays the segments in a pie chart.

## Signature

```python
obj.Mode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePieChartSliceEdgeModeNone` | 0 | No frame |
| `ePieChartSliceEdgeModeAutomatic` | 1 | Automatic frame |

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
oMySettings.SliceEdge.Mode = dd.ePieChartSliceEdgeModeNone
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Mode_IRepPieChartSliceEdgeInt.htm`*
