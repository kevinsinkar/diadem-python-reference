---
title: "IRepPieChartCurveInt.ValueMode"
description: "Specifies whether DIAdem takes the values of the segments from a channel or uses the values you enter with the Value for PieChartSlice property in a pie chart i"
---

# IRepPieChartCurveInt.ValueMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ValueMode for PieChartCurve

Specifies whether DIAdem takes the values of the segments from a channel or uses the values you enter with the Value for PieChartSlice property in a pie chart in DIAdem REPORT. DIAdem saves the values you enter in the layout.

## Signature

```python
obj.ValueMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePieChartValueModeChannel` | 0 | Taken from channel |
| `ePieChartValueModeLayout` | 1 | Entered |

## Python example

```python
oMyPieChart = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPieChart, "PieChart")
oMyPieChart.CurvePieChart.ValueMode= dd.ePieChartValueModeLayout
oMySlices = oMyPieChart.CurvePieChart.Slices
oMySlices.Count = 5
for i in range( 1, oMySlices.Count+1):
    oMySlices(i).Value = i
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ValueMode_IRepPieChartCurveInt.htm`*
