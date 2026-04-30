---
title: "IRepD3SelectedSubObjInt.Name"
description: "Specifies the name of a selected element in a 3D axis system in DIAdem REPORT."
---

# IRepD3SelectedSubObjInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for 3DSelectedElement

Specifies the name of a selected element in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for i in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection(i).Type + "\t" + "Element name: " + oMySelection(i).Name + "\r\n"
        print(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepD3SelectedSubObjInt.htm`*
