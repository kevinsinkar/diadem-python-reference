---
title: "IRepSheetListInt.Item"
description: "Returns the worksheet associated with a specific name or a specific index in DIAdem REPORT."
---

# IRepSheetListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for Sheets

Returns the worksheet associated with a specific name or a specific index in DIAdem REPORT.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
dd.Report.Sheets.Item(1).Name = "Default"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepSheetListInt.htm`*
