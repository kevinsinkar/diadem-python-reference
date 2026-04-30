---
title: "IRepPaletteColorListInt.Item"
description: "Returns the palette color settings associated with a specific name or a specific index, in DIAdem REPORT."
---

# IRepPaletteColorListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for TablePaletteColors

Returns the palette color settings associated with a specific name or a specific index, in DIAdem REPORT.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
dd.Report.NewLayout()
oMyReportObj = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable, "My2DTable")
oMyPos = oMyReportObj.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCol = oMyReportObj.Columns.Add(dd.e2DTableColumnChannel)
oMyCol.Channel.Reference = "[1]/[1]"
oMyCol.Settings.Font.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyReportObj.Settings.Palette
oMyPalette.Count = 3
for i in range( 1, oMyPalette.Count+1):
    oMyPalette.Item(i).Color.SetPredefinedColor(i)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepPaletteColorListInt.htm`*
