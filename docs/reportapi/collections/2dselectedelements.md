---
title: "2DSelectedElements"
description: "Collection of all 2DSelectedElement objects in DIAdem REPORT. Use the 2DSelectedElements collection to access a selected element in a 2D axis system."
---

# 2DSelectedElements

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 2DSelectedElements

Collection of all 2DSelectedElement objects in DIAdem REPORT. Use the 2DSelectedElements collection to access a selected element in a 2D axis system.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for I in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2selectedsubobjectslistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd2selectedsubobjectslistint-add2d/">Add2D</a> | <a href="../../methods/irepd2selectedsubobjectslistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-selectedelements/">SelectedElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2SelectedSubObjectsListInt.htm`*
