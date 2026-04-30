---
title: "IRepD3SelectedSubObjInt"
description: "The 3DSelectedElement object provides a selected element in a 3D axis system in DIAdem REPORT."
---

# IRepD3SelectedSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DSelectedElement

The 3DSelectedElement object provides a selected element in a 3D axis system in DIAdem REPORT.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for i in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3selectedsubobjint-name/">Name</a> | <a href="../../properties/irepd3selectedsubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/3dselectedelements/">3DSelectedElements</a>.<a href="../../methods/irepd3selectedsubobjectslistint-add3d/">Add3D</a> | <a href="../../collections/3dselectedelements/">3DSelectedElements</a>.<a href="../../methods/irepd3selectedsubobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3SelectedSubObjInt.htm`*
