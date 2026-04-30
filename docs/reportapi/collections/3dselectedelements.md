---
title: "3DSelectedElements"
description: "Collection of all 3DSelectedElement objects in DIAdem REPORT. Use the 3DSelectedElements collection to access a selected element in a 3D axis system."
---

# 3DSelectedElements

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 3DSelectedElements

Collection of all 3DSelectedElement objects in DIAdem REPORT. Use the 3DSelectedElements collection to access a selected element in a 3D axis system.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for I in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3selectedsubobjectslistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd3selectedsubobjectslistint-add3d/">Add3D</a> | <a href="../../methods/irepd3selectedsubobjectslistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd3axisint/">3DAxisSystem</a>.<a href="../../properties/irepd3axisint-selectedelements/">SelectedElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3SelectedSubObjectsListInt.htm`*
