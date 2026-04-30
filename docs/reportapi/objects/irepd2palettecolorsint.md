---
title: "IRepD2PaletteColorsInt"
description: "The 2DPaletteColors object provides the color palette in a 2D axis system in the display mode Grouped bars or Stacked bars in DIAdem REPORT."
---

# IRepD2PaletteColorsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DPaletteColors

The 2DPaletteColors object provides the color palette in a 2D axis system in the display mode Grouped bars or Stacked bars in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")

oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeGroupedBars, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = ""
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.Settings.DisplayMode = dd.eBarsDisplayMode2D
oMy2DCurve.Shape.Settings.Filling.Color.ColorIndex = dd.eColorIndexPalette
oMy2DCurve.Shape.Settings.BorderLine.Color.ColorIndex = dd.eColorIndexPalette

oMyPaletteColors = oMy2DCurve.Shape.Settings.Palette.Colors
oMyPaletteColors(1).ColorIndex = dd.eColorIndexDarkYellow
oMyPaletteColors(2).ColorIndex = dd.eColorIndexBlue
oMyPaletteColors(1).Transparency = 10

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2palettecolorsint-colors/">Colors</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjboxwhiskersettingsint/">2DBoxWhiskerSettings</a>.<a href="../../properties/irepd2shapeobjboxwhiskersettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjbarsgroupedsettingsint/">2DGroupedBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjbarsstackedsettingsint/">2DStackedBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarsstackedsettingsint-palette/">Palette</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2PaletteColorsInt.htm`*
