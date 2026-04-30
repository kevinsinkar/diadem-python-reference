---
title: "3DTableSelectedElements"
description: "Collection of all 3DTableSelectedElement objects in DIAdem REPORT. Use the 3DTableSelectedElements collection to access a selected element in a 3D table."
---

# 3DTableSelectedElements

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 3DTableSelectedElements

Collection of all 3DTableSelectedElement objects in DIAdem REPORT. Use the 3DTableSelectedElements collection to access a selected element in a 3D table.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DTable :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMyReportObj.SelectedElements.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable3dselectedsubobjectslistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptable3dselectedsubobjectslistint-add3dtable/">Add3DTable</a> | <a href="../../methods/ireptable3dselectedsubobjectslistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ireptable3dint/">3DTable</a>.<a href="../../properties/ireptable3dint-selectedelements/">SelectedElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable3DSelectedSubObjectsListInt.htm`*
