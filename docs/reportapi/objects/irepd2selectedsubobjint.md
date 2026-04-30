---
title: "IRepD2SelectedSubObjInt"
description: "The 2DSelectedElement object provides a selected element in a 2D axis system in DIAdem REPORT."
---

# IRepD2SelectedSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DSelectedElement

The 2DSelectedElement object provides a selected element in a 2D axis system in DIAdem REPORT.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for i in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2selectedsubobjint-name/">Name</a> | <a href="../../properties/irepd2selectedsubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dselectedelements/">2DSelectedElements</a>.<a href="../../methods/irepd2selectedsubobjectslistint-add2d/">Add2D</a> | <a href="../../collections/2dselectedelements/">2DSelectedElements</a>.<a href="../../methods/irepd2selectedsubobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2SelectedSubObjInt.htm`*
