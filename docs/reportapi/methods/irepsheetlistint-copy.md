---
title: "IRepSheetListInt.Copy"
description: "Copies a worksheet to a specified position in DIAdem REPORT."
---

# IRepSheetListInt.Copy

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Copy for Sheets

Copies a worksheet to a specified position in DIAdem REPORT.

## Signature

```python
return_value = obj.Copy(NameOrIndex, NewName, InsertBeforeNameOrIndex)
```

## Python example

```python
oMyFirstSheet = dd.Report.ActiveSheet
oMyNewSheet = dd.Report.Sheets.Copy(2,"Sheet1",1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Copy_IRepSheetListInt.htm`*
