---
title: "IRepPieChartSelectedSubObjInt"
description: "The PieChartSelectedElement object provides a selected element of a pie chart in DIAdem REPORT."
---

# IRepPieChartSelectedSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PieChartSelectedElement

The PieChartSelectedElement object provides a selected element of a pie chart in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppiechartselectedsubobjint-name/">Name</a> | <a href="../../properties/ireppiechartselectedsubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/piechartselectedelements/">PieChartSelectedElements</a>.<a href="../../methods/ireppiechartselectedsubobjectslistint-addpiechart/">AddPieChart</a> | <a href="../../collections/piechartselectedelements/">PieChartSelectedElements</a>.<a href="../../methods/ireppiechartselectedsubobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPieChartSelectedSubObjInt.htm`*
