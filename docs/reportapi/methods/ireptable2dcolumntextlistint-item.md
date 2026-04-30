---
title: "IRepTable2DColumnTextListInt.Item"
description: "Returns the text list of a 2D table associated with a specific name or a specific index in DIAdem REPORT."
---

# IRepTable2DColumnTextListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for 2DTableColumnTextList

Returns the text list of a 2D table associated with a specific name or a specific index in DIAdem REPORT.

## Signature

```python
return_value = obj.Item(Index)
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
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMy2DTable.Position.ByBorder.Top = 30
oMy2DTable.Position.ByBorder.Bottom = 20
oMy2DTable.Position.ByBorder.Left = 20
oMy2DTable.Position.ByBorder.Right = 30
oMy2DTable.Columns.Add(dd.e2DTableColumnText)
oMyTextList = oMy2DTable.Columns(1).TextList
oMyTextList.Count = 10
for I in range( 1, oMyTextList.Count+1):
    oMyTextList.Item(I).Text = "Text no: " + I
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepTable2DColumnTextListInt.htm`*
