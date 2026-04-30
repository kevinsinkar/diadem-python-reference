---
title: "IRepPieChartSelectedSubObjInt.Name"
description: "Specifies the name of the selected object in a pie chart in DIAdem REPORT."
---

# IRepPieChartSelectedSubObjInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for PieChartSelectedElement

Specifies the name of the selected object in a pie chart in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPieChart :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for I in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepPieChartSelectedSubObjInt.htm`*
