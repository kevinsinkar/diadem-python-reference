---
title: "IRepD3SelectedSubObjectsListInt.Count"
description: "Returns the number of elements selected in a 3D axis system in DIAdem REPORT."
---

# IRepD3SelectedSubObjectsListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 3DSelectedElements

Returns the number of elements selected in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
sOutput = ""
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of selected elements: " + oMyReportObj.SelectedElements.Count)
        for oMySelection in oMyReportObj.SelectedElements:
            sOutput = sOutput + "Element type: " + oMySelection.Type + "\t" + "Element name: " + oMySelection.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepD3SelectedSubObjectsListInt.htm`*
