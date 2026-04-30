---
title: "IRepPieChartSliceLabelInt.Channel"
description: "Specifies the channel from which DIAdem REPORT takes the label texts in a pie chart. DIAdem only uses the property Channel if you assign the value True to the p"
---

# IRepPieChartSliceLabelInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for PieChartSliceLabel

Specifies the channel from which DIAdem REPORT takes the label texts in a pie chart. DIAdem only uses the property Channel if you assign the value True to the property CategoryVisible and the value eCategoryModeChannel to the property CategoryMode .

## Signature

```python
return_value = obj.Channel
```

## Python example

```python
oPieChart = dd.Report.ActiveSheet.Objects("PieChart1")
oPieChart.CurvePieChart.Channel.Reference = "[5]/[3]"
oPieChart.CurvePieChart.SliceLabel.Channel.Reference = "[5]/[1]"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepPieChartSliceLabelInt.htm`*
