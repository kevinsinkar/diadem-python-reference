---
title: "IRepPieChartSliceEdgeInt"
description: "The PieChartSliceEdge object provides the slice frame in a pie chart in DIAdem REPORT."
---

# IRepPieChartSliceEdgeInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PieChartSliceEdge

The PieChartSliceEdge object provides the slice frame in a pie chart in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppiechartsliceedgeint-mode/">Mode</a> | <a href="../../properties/ireppiechartsliceedgeint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppiechartsettingsint/">PieChartSettings</a>.<a href="../../properties/ireppiechartsettingsint-sliceedge/">SliceEdge</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPieChartSliceEdgeInt.htm`*
