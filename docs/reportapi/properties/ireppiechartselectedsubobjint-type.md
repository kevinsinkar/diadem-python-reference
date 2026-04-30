---
title: "IRepPieChartSelectedSubObjInt.Type"
description: "Specifies the type of the selected element of a pie chart in DIAdem REPORT."
---

# IRepPieChartSelectedSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for PieChartSelectedElement

Specifies the type of the selected element of a pie chart in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePieChartElementMain` | 0 | Main object |
| `ePieChartElementSlice` | 1 | Segment |
| `ePieChartElementLabel` | 2 | Segment label |
| `ePieChartElementLegend` | 3 | Legend |

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
oMyCurvePieChart = oMyPieChart.CurvePieChart # CurvePieChartPieChart
oMyCurvePieChart.Channel.Reference = "[5]/[4]"
dd.Report.Refresh()
oMySelectedElement = oMyPieChart.SelectedElements.AddPieChart(dd.ePieChartElementSlice, 2)
print("Selected element: " , TypeAsText(oMySelectedElement.Type))

#Function to convert type into text
def TypeAsText(eMyType):
    select_variable_0 = eMyType
    if (select_variable_0 == dd.ePieChartElementMain) :
        TypeAsText = "Pie chart"
    elif (select_variable_0 == dd.ePieChartElementSlice) :
        TypeAsText = "Segment"
    elif (select_variable_0 == dd.ePieChartElementLabel) :
        TypeAsText = "Label"
    elif (select_variable_0 == dd.ePieChartElementLegend) :
        TypeAsText = "Legend"
    return TypeAsText
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepPieChartSelectedSubObjInt.htm`*
