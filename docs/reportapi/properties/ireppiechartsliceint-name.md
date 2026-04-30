---
title: "IRepPieChartSliceInt.Name"
description: "Specifies the name of a segment in a pie chart in DIAdem REPORT."
---

# IRepPieChartSliceInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for PieChartSlice

Specifies the name of a segment in a pie chart in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPieChart :
        for oMySlice in oMyReportObj.CurvePieChart.Slices:
            sOutput = sOutput + "Object " + oMySlice.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepPieChartSliceInt.htm`*
