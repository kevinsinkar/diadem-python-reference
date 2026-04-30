---
title: "IRepTable2DColumnListInt.Remove"
description: "Deletes a column from a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnListInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for 2DTableColumns

Deletes a column from a 2D table in DIAdem REPORT.

## Signature

```python
obj.Remove(Index)
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        iColumnCount = oMyReportObj.Columns.Count
        if iColumnCount > 1 :
            oMyReportObj.Columns.Remove(iColumnCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepTable2DColumnListInt.htm`*
