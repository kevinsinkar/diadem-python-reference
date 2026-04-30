---
title: "IRepSheetListInt.Exists"
description: "Checks whether a worksheet with a specific name already exists in DIAdem REPORT."
---

# IRepSheetListInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for Sheets

Checks whether a worksheet with a specific name already exists in DIAdem REPORT.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
if not dd.Report.Sheets.Exists("MySheet") :
    dd.Report.Sheets.Add("MySheet")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Exists_IRepSheetListInt.htm`*
