---
title: "IRepTable2DSelectedSubObjInt.ColumnIndex"
description: "Specifies the index of a selected column in a 2D table in DIAdem REPORT."
---

# IRepTable2DSelectedSubObjInt.ColumnIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColumnIndex for 2DTableSelectedElement

Specifies the index of a selected column in a 2D table in DIAdem REPORT.

## Signature

```python
obj.ColumnIndex
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of selected elements: " + oMyReportObj.SelectedElements.Count)
        for oMySelection in oMyReportObj.SelectedElements:
            sOutput = sOutput + "Element type: " + oMySelection.Type
            sOutput = sOutput + "; Column index: " + oMySelection.ColumnIndex + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColumnIndex_IRepTable2DSelectedSubObjInt.htm`*
