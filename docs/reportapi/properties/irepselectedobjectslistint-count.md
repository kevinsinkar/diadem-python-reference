---
title: "IRepSelectedObjectsListInt.Count"
description: "Returns the number of the selected objects in DIAdem REPORT."
---

# IRepSelectedObjectsListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for SelectedObjects

Returns the number of the selected objects in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObj = dd.Report.SelectedObjects()
if dd.MsgBoxDisp("Number of selected objects== " + oMyReportObj.Count + "\r\n" + "Do you want to remove selection?","MB_YESNO","MsgTypeNote") == "IDYes" :
    oMyReportObj.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepSelectedObjectsListInt.htm`*
