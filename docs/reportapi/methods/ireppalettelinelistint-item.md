---
title: "IRepPaletteLineListInt.Item"
description: "Returns the palette color settings associated with a specific index, for the curve display in a 2D axis system in DIAdem REPORT."
---

# IRepPaletteLineListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for PaletteLines

Returns the palette color settings associated with a specific index, for the curve display in a 2D axis system in DIAdem REPORT.

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
oMyReportObj = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMyReportObj.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyReportObj.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLine = oMyCurve.Shape.Settings.Line
oMyLine.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyCurve.Shape.Settings.Palette.Lines
for i in range( 1, oMyPalette.Count+1):
    oMyPalette.Item(i).Color.SetPredefinedColor(i)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepPaletteLineListInt.htm`*
