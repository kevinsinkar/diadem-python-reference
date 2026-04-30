---
title: "IRepSheetListInt.Insert"
description: "Inserts a new worksheet into DIAdem REPORT."
---

# IRepSheetListInt.Insert

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Insert for Sheets

Inserts a new worksheet into DIAdem REPORT.

## Signature

```python
return_value = obj.Insert(Name, InsertBeforeNameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <a href="../../../scriptview/methods/itosheetcontint-add/">Add</a> method to add a new worksheet behind the last worksheet.</td></tr></table>
</div>

## Python example

```python
CallReport.Sheets.Insert("MyNewSheet", 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Insert_IRepSheetListInt.htm`*
