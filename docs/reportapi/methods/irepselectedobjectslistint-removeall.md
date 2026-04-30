---
title: "IRepSelectedObjectsListInt.RemoveAll"
description: "Deselects all selected objects in DIAdem REPORT."
---

# IRepSelectedObjectsListInt.RemoveAll

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: RemoveAll for SelectedObjects

Deselects all selected objects in DIAdem REPORT.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyReportObj = dd.Report.SelectedObjects()
if oMyReportObj.Count > 0 :
    if dd.MsgBoxDisp("Number of selected object== " + oMyReportObj.Count + "\r\n" + "Do you want to remove selection?","MB_YesNo","MsgTypeNote") == "IDYes" :
        oMyReportObj.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_RemoveAll_IRepSelectedObjectsListInt.htm`*
