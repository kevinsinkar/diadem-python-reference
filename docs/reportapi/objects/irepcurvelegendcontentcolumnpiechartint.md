---
title: "IRepCurvelegendContentColumnPieChartInt"
description: "The CurveLegendColumn object provides the properties of a column of a curve legend"
---

# IRepCurvelegendContentColumnPieChartInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CurveLegendColumnPieChart

The CurveLegendColumn object provides the properties of a column of a curve legend

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPieChart :
        oMyReportObj.CurveLegend.Columns.RemoveAll()
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
oMySliceLabel = oMyCurvePieChart.SliceLabel
oMySliceLabel.CategoryVisible = True
oMySliceLabel.Channel.Reference = "[5]/[1]"
oMySliceLabel.CategoryMode = dd.eCategoryModeChannel
oMyLegend = oMyPieChart.Legend
oMyLegend.Visible = True
oMyCurveLegendPos = oMyLegend.Position
oMyCurveLegendPos.RelativePosition = dd.eLegendRelativePositionTopLeft
oMyCurveLegendPos.SizeMode = dd.eLegendSizeElementwise
oMyCurveLegendPos.ElementHeight = 5
oMyCurveLegendPos.ElementWidth = 35
oMyLegend.Settings.Font.Size = 4
oMyLegendColumns = oMyLegend.Columns
oMyLegendColumns.Add()
oMyLegendColumns(1).Title = "First title"
oMyLegendColumns(1).Type = dd.eLegendTextPieChartCustomText
oMyLegendColumns(1).RelativeWidth = 2
oMyLegendColumns(1).Text = "First col - longer text"
oMyLegendColumns(2).Title = "Second title"
oMyLegendColumns(2).Type = dd.eLegendTextPieChartSliceRelatedText
oMyLegendColumns(2).RelativeWidth = 2
oMyLegendColumns(2).Text = "Second col"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/irepcurvelegendcontentcolumnpiechartint-relativewidth/">RelativeWidth</a> | <a href="../../properties/irepcurvelegendcontentcolumnpiechartint-text/">Text</a> | <a href="../../properties/irepcurvelegendcontentcolumnpiechartint-title/">Title</a> | <a href="../../properties/irepcurvelegendcontentcolumnpiechartint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/curvelegendcolumns/">CurveLegendColumns</a>.<a href="../../methods/irepcurvelegendcontentcolumnslistint-add/">Add</a> | <a href="../../collections/curvelegendcolumns/">CurveLegendColumns</a>.<a href="../../methods/irepcurvelegendcontentcolumnslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCurvelegendContentColumnPieChartInt.htm`*
