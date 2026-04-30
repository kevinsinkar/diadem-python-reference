---
title: "IRepBaseCtrlInt.IsSelected"
description: "Specifies whether an object is selected in DIAdem REPORT."
---

# IRepBaseCtrlInt.IsSelected

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IsSelected for ReportObject

Specifies whether an object is selected in DIAdem REPORT.

## Signature

```python
obj.IsSelected
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.IsSelected :
        oMyReportObj.TagStored = "Selected"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IsSelected_IRepBaseCtrlInt.htm`*
