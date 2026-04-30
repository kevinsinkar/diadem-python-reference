---
title: "PieChartSelectedElements"
description: "Collection of all PieChartSelectedElement objects in DIAdem REPORT. Use the PieChartSelectedElements collection to access a selected element in a pie chart."
---

# PieChartSelectedElements

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: PieChartSelectedElements

Collection of all PieChartSelectedElement objects in DIAdem REPORT. Use the PieChartSelectedElements collection to access a selected element in a pie chart.

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
<p><a href="../../properties/ireppiechartselectedsubobjectslistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireppiechartselectedsubobjectslistint-addpiechart/">AddPieChart</a> | <a href="../../methods/ireppiechartselectedsubobjectslistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ireppiechartint/">PieChart</a>.<a href="../../properties/ireppiechartint-selectedelements/">SelectedElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPieChartSelectedSubObjectsListInt.htm`*
