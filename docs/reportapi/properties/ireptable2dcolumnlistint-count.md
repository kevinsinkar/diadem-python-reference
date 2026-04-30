---
title: "IRepTable2DColumnListInt.Count"
description: "Returns the number of columns in a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 2DTableColumns

Returns the number of columns in a 2D table in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of columns: " + oMyReportObj.Columns.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepTable2DColumnListInt.htm`*
