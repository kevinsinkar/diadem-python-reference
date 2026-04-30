---
title: "TablePaletteColors"
description: "Collection of all TablePaletteColor objects in DIAdem REPORT. Use the TablePaletteColors collection to delete the palette colors for the 2D table display or to "
---

# TablePaletteColors

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: TablePaletteColors

Collection of all TablePaletteColor objects in DIAdem REPORT. Use the TablePaletteColors collection to delete the palette colors for the 2D table display or to add new palette colors.

## Python example

```python
dd.Report.NewLayout()
oMyReportObj = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable, "My2DTable")
oMyPosition = oMyReportObj.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyColumn = oMyReportObj.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[1]"
oMyColumn.Settings.Font.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyReportObj.Settings.Palette
oMyPalette.Count = 3
for i in range( 1, oMyPalette.Count+1):
    oMyPalette(i).Color.SetPredefinedColor(i)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppalettecolorlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireppalettecolorlistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-palette/">Palette</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPaletteColorListInt.htm`*
