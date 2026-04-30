---
title: "IRepSheetListInt.Add"
description: "Generates a new worksheet in DIAdem REPORT."
---

# IRepSheetListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for Sheets

Generates a new worksheet in DIAdem REPORT.

## Signature

```python
return_value = obj.Add(Name)
```

## Python example

```python
oMySheets = dd.Report.Sheets
oMySheets.RemoveAll()
oMySheets.Add("Sheet 1")
oMySheets.Add("Sheet 2")
oMySheets.Add("Sheet 3")
oMySheets.Add("Sheet 4")
dd.Report.Sheets.Move(5 ,"Sheet 1")
dd.Report.Sheets.Move("Sheet 3" ,"Sheet 1")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepSheetListInt.htm`*
