---
title: "IRepPieChartSliceLabelInt"
description: "The PieChartSliceLabel object provides the slice labels in a pie chart in DIAdem REPORT."
---

# IRepPieChartSliceLabelInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PieChartSliceLabel

The PieChartSliceLabel object provides the slice labels in a pie chart in DIAdem REPORT.

## Python example

```python
oPieChart = dd.Report.ActiveSheet.Objects("PieChart1")
oPieChart.CurvePieChart.Channel.Reference = "[5]/[3]"
oPieChart.CurvePieChart.SliceLabel.Channel.Reference = "[5]/[1]"
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
oMyCurvePieChart.SliceLabel.CategoryVisible = False
oMySettings = oMyPieChart.Settings
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppiechartslicelabelint-categorymode/">CategoryMode</a> | <a href="../../properties/ireppiechartslicelabelint-categoryvisible/">CategoryVisible</a> | <a href="../../properties/ireppiechartslicelabelint-channel/">Channel</a> | <a href="../../properties/ireppiechartslicelabelint-font/">Font</a> | <a href="../../properties/ireppiechartslicelabelint-physicalvalueformat/">PhysicalValueFormat</a> | <a href="../../properties/ireppiechartslicelabelint-physicalvaluevisible/">PhysicalValueVisible</a> | <a href="../../properties/ireppiechartslicelabelint-relativeposition/">RelativePosition</a> | <a href="../../properties/ireppiechartslicelabelint-relativevalueformat/">RelativeValueFormat</a> | <a href="../../properties/ireppiechartslicelabelint-relativevaluevisible/">RelativeValueVisible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppiechartcurveint/">PieChartCurve</a>.<a href="../../properties/ireppiechartcurveint-slicelabel/">SliceLabel</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPieChartSliceLabelInt.htm`*
