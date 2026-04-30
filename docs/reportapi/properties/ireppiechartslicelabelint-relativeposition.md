---
title: "IRepPieChartSliceLabelInt.RelativePosition"
description: "Specifies the relative position of the slice labels in a pie chart in DIAdem REPORT."
---

# IRepPieChartSliceLabelInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for PieChartSliceLabel

Specifies the relative position of the slice labels in a pie chart in DIAdem REPORT.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePieChartLabelPositionManual` | 0 | Move manually, no automatic alignment. |
| `ePieChartLabelPositionCentered` | 1 | Centered over the segment. |
| `ePieChartLabelPositionInside` | 2 | Within the circle diagram, as far outside as possible. |
| `ePieChartLabelPositionOutside` | 3 | Outside the pie chart. |

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
oMySliceLabel = oMyCurvePieChart.SliceLabel
oMySliceLabel.CategoryVisible = True
oMySliceLabel.Channel.Reference = "[5]/[1]"
oMySliceLabel.CategoryMode = dd.eCategoryModeChannel
oMySliceLabel.RelativePosition = dd.ePieChartLabelPositionOutside
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepPieChartSliceLabelInt.htm`*
