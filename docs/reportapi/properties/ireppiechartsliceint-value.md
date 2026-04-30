---
title: "IRepPieChartSliceInt.Value"
description: "Specifies the value of a pie chart segment in DIAdem REPORT. DIAdem only includes this value if you have assigned the ePieChartValueModeLayout value to the Valu"
---

# IRepPieChartSliceInt.Value

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Value for PieChartSlice

Specifies the value of a pie chart segment in DIAdem REPORT. DIAdem only includes this value if you have assigned the ePieChartValueModeLayout value to the ValueMode for PieChartCurve property. DIAdem saves the values you enter in the layout.

## Signature

```python
obj.Value
```

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

*Source: `ReportApi/properties/Report_property_Value_IRepPieChartSliceInt.htm`*
