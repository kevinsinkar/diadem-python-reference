---
title: "IRepPaletteColorInt"
description: "The TablePaletteColor object provides a palette color for the 2D table display in DIAdem REPORT."
---

# IRepPaletteColorInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: TablePaletteColor

The TablePaletteColor object provides a palette color for the 2D table display in DIAdem REPORT.

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
<p><a href="../../properties/ireppalettecolorint-color/">Color</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/tablepalettecolors/">TablePaletteColors</a>.<a href="../../methods/ireppalettecolorlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPaletteColorInt.htm`*
