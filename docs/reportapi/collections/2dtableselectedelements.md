---
title: "2DTableSelectedElements"
description: "Collection of all 2DTableSelectedElement objects in DIAdem REPORT. Use the 2DTableSelectedElements collection to access a selected element in a 2D table."
---

# 2DTableSelectedElements

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 2DTableSelectedElements

Collection of all 2DTableSelectedElement objects in DIAdem REPORT. Use the 2DTableSelectedElements collection to access a selected element in a 2D table.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMyReportObj.SelectedElements.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dselectedsubobjectslistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptable2dselectedsubobjectslistint-add2dtable/">Add2DTable</a> | <a href="../../methods/ireptable2dselectedsubobjectslistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ireptable2dint/">2DTable</a>.<a href="../../properties/ireptable2dint-selectedelements/">SelectedElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DSelectedSubObjectsListInt.htm`*
