---
title: "IRepPieChartSliceInt"
description: "The PieChartSlice object provides a slice in a pie chart in DIAdem REPORT."
---

# IRepPieChartSliceInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PieChartSlice

The PieChartSlice object provides a slice in a pie chart in DIAdem REPORT.

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
oMyCurvePieChart.Slices(2).Enable = False
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppiechartsliceint-enable/">Enable</a> | <a href="../../properties/ireppiechartsliceint-explosion/">Explosion</a> | <a href="../../properties/ireppiechartsliceint-filleffects/">FillEffects</a> | <a href="../../properties/ireppiechartsliceint-name/">Name</a> | <a href="../../properties/ireppiechartsliceint-value/">Value</a> | <a href="../../properties/ireppiechartsliceint-visibleinlegend/">VisibleInLegend</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/piechartslices/">PieChartSlices</a>.<a href="../../methods/ireppiechartslicesint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPieChartSliceInt.htm`*
