---
title: "IRepPieChartCurveInt"
description: "The PieChartCurve object provides a slice in a pie chart in DIAdem REPORT."
---

# IRepPieChartCurveInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PieChartCurve

The PieChartCurve object provides a slice in a pie chart in DIAdem REPORT.

## Python example

```python
oPieChart = dd.Report.ActiveSheet.Objects("PieChart1")
oPieChart.CurvePieChart.Channel.Reference = "[5]/[3]"
```

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppiechartcurveint-channel/">Channel</a> | <a href="../../properties/ireppiechartcurveint-slicelabel/">SliceLabel</a> | <a href="../../properties/ireppiechartcurveint-slices/">Slices</a> | <a href="../../properties/ireppiechartcurveint-valuemode/">ValueMode</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppiechartint/">PieChart</a>.<a href="../../properties/ireppiechartint-curvepiechart/">CurvePieChart</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPieChartCurveInt.htm`*
