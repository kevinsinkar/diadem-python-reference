---
title: "IRepTable3DSelectedSubObjInt"
description: "The 3DTableSelectedElement object provides a selected element of a 3D table in DIAdem REPORT."
---

# IRepTable3DSelectedSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DTableSelectedElement

The 3DTableSelectedElement object provides a selected element of a 3D table in DIAdem REPORT.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DTable :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for i in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable3dselectedsubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/3dtableselectedelements/">3DTableSelectedElements</a>.<a href="../../methods/ireptable3dselectedsubobjectslistint-add3dtable/">Add3DTable</a> | <a href="../../collections/3dtableselectedelements/">3DTableSelectedElements</a>.<a href="../../methods/ireptable3dselectedsubobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable3DSelectedSubObjInt.htm`*
