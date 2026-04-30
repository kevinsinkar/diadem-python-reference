---
title: "IRepCurvelegendContentColumnPieChartInt.Type"
description: "Specifies whether DIAdem labels the legend of a pie chart with user defined text or with default text. With a free text you can use a DIAdem expression to displ"
---

# IRepCurvelegendContentColumnPieChartInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for CurveLegendColumnPieChart

Specifies whether DIAdem labels the legend of a pie chart with user defined text or with default text. With a free text you can use a DIAdem expression to display for example the relative or absolute values of the segments: @@ CurrRelValue @@ or @@ CurrAbsValue @@ .

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendTextPieChartCustomText` | 6 | Free text—DIAdem uses the label text you enter for all legend symbols. |
| `eLegendTextPieChartSliceRelatedText` | 7 | Segment-related text—DIAdem labels each legend symbol with the free text you enter. |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm", "TDM", "Load|ChnXYRelation")
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
oMySliceLabel.Channel.Reference = "[5]/[1]"
oMySliceLabel.CategoryMode = dd.eCategoryModeChannel
oMyLegend = oMyPieChart.Legend
oMyLegend.Visible = True
oMyLegend.Frame.Color.SetRGBColor(dd.RGB(198,198,198))
oMyCurveLegendPos = oMyLegend.Position
oMyCurveLegendPos.RelativePosition = dd.eLegendRelativePositionTopLeft
oMyCurveLegendPos.SizeMode = dd.eLegendSizeElementwise
oMyCurveLegendPos.ElementHeight = 5
oMyCurveLegendPos.ElementWidth = 35
oMyLegend.Settings.PortionSymbolField = 18
oMyLegendColumns = oMyLegend.Columns
oMyLegendColumns.Add()
oMyLegendColumns(1).Type = dd.eLegendTextPieChartCustomText
oMyLegendColumns(1).Title = "Value"
oMyLegendColumns(1).RelativeWidth = 1
oMyLegendColumns(1).Text = "@@CurrAbsValue@@"
oMyLegendColumns(2).Type = dd.eLegendTextPieChartSliceRelatedText
oMyLegendColumns(2).Title = "Slice Label"
oMyLegendColumns(2).RelativeWidth = 3
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepCurvelegendContentColumnPieChartInt.htm`*
