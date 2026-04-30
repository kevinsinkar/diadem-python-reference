---
title: "IRepTable2DSelectedSubObjInt.Type"
description: "Specifies the type of a selected subobject in a 2D table in DIAdem REPORT."
---

# IRepTable2DSelectedSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 2DTableSelectedElement

Specifies the type of a selected subobject in a 2D table in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of selected elements: " + oMyReportObj.SelectedElements.Count)
        for oMySelection in oMyReportObj.SelectedElements:
            sOutput = sOutput + "Element type: " + oMySelection.Type + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepTable2DSelectedSubObjInt.htm`*
