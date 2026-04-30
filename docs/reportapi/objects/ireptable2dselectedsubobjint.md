---
title: "IRepTable2DSelectedSubObjInt"
description: "The 2DTableSelectedElement object provides a selected element from a 2D table in DIAdem REPORT."
---

# IRepTable2DSelectedSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableSelectedElement

The 2DTableSelectedElement object provides a selected element from a 2D table in DIAdem REPORT.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for I in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dselectedsubobjint-columnindex/">ColumnIndex</a> | <a href="../../properties/ireptable2dselectedsubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dtableselectedelements/">2DTableSelectedElements</a>.<a href="../../methods/ireptable2dselectedsubobjectslistint-add2dtable/">Add2DTable</a> | <a href="../../collections/2dtableselectedelements/">2DTableSelectedElements</a>.<a href="../../methods/ireptable2dselectedsubobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DSelectedSubObjInt.htm`*
