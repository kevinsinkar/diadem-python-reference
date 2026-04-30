---
title: "PaletteLines"
description: "Collection of all PaletteLine objects in DIAdem REPORT. Use the PaletteLines collection to delete the palette color for the line display in a 2D axis system or "
---

# PaletteLines

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: PaletteLines

Collection of all PaletteLine objects in DIAdem REPORT. Use the PaletteLines collection to delete the palette color for the line display in a 2D axis system or to add new palette colors.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLine = oMyCurve.Shape.Settings.Line
oMyLine.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyCurve.Shape.Settings.Palette.Lines
for i in range( 1, oMyPalette.Count+1):
    oMyPalette.Item(i).Color.SetPredefinedColor(i)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppalettelinelistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireppalettelinelistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd2paletteint/">2DPalette</a>.<a href="../../properties/irepd2paletteint-lines/">Lines</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPaletteLineListInt.htm`*
