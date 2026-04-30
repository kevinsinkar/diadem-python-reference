---
title: "IRepPaletteLineColorInt.Transparency"
description: "Specifies the transparency of a palette color as a percentage in DIAdem REPORT. The value 100 specifies a completely transparent display and the value 0 specifi"
---

# IRepPaletteLineColorInt.Transparency

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Transparency for PaletteColor

Specifies the transparency of a palette color as a percentage in DIAdem REPORT. The value 100 specifies a completely transparent display and the value 0 specifies a completely opaque display. Not all DIAdem objects display transparency.

## Signature

```python
obj.Transparency
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Transparency_IRepPaletteLineColorInt.htm`*
