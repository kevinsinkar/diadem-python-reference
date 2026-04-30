---
title: "IRepBaseCtrlInt.Select"
description: "Selects an object in DIAdem REPORT."
---

# IRepBaseCtrlInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for ReportObject

Selects an object in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.TagStored == "Selected" :
        oMyReportObj.Select()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepBaseCtrlInt.htm`*
