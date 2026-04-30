---
title: "IRepCtrlListInt.Remove"
description: "Deletes an object in DIAdem REPORT."
---

# IRepCtrlListInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for ReportObjects

Deletes an object in DIAdem REPORT.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.IsSelected :
        oMyReportObjects.Remove(oMyReportObj.Index)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepCtrlListInt.htm`*
