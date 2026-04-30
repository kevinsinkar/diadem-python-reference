---
title: "IRepPolarSelectedSubObjectsListInt.Count"
description: "Returns the number of elements selected in a polar axis system in DIAdem REPORT."
---

# IRepPolarSelectedSubObjectsListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for PolarSelectedElements

Returns the number of elements selected in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
sOutput = ""
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        oMySelection = oMyReportObj.SelectedElements
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of selected elements: " + oMySelection.Count)
        for i in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\t" + "Element name: " + oMySelection.Item(i).Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepPolarSelectedSubObjectsListInt.htm`*
