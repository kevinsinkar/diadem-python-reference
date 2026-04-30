---
title: "IRepSheetListInt.Remove"
description: "Deletes a worksheet in DIAdem REPORT."
---

# IRepSheetListInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for Sheets

Deletes a worksheet in DIAdem REPORT.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
iSheetCount = dd.Report.Sheets.Count
if iSheetCount > 1 :
    dd.Report.Sheets.Remove(iSheetCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepSheetListInt.htm`*
