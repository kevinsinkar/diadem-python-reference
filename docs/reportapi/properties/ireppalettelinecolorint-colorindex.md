---
title: "IRepPaletteLineColorInt.ColorIndex"
description: "Uses predefined colors in DIAdem REPORT to specify the color. For user-defined colors, select the value eColorIndexOtherColors , and use the RGB property or the"
---

# IRepPaletteLineColorInt.ColorIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColorIndex for PaletteColor

Uses predefined colors in DIAdem REPORT to specify the color. For user-defined colors, select the value eColorIndexOtherColors , and use the RGB property or the SetRGBColor method to select the color.

## Signature

```python
obj.ColorIndex
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorIndexNone` | 0 | None |
| `eColorIndexBlack` | 1 | Black |
| `eColorIndexRed` | 2 | Red |
| `eColorIndexGreen` | 3 | Green |
| `eColorIndexBlue` | 4 | Blue |
| `eColorIndexViolet` | 5 | Violet |
| `eColorIndexTurquoise` | 6 | Turquoise |
| `eColorIndexGrey` | 7 | Gray |
| `eColorIndexYellow` | 8 | Yellow |
| `eColorIndexDarkRed` | 9 | Dark red |
| `eColorIndexDarkGreen` | 10 | Dark green |
| `eColorIndexDarkBlue` | 11 | Dark blue |
| `eColorIndexDarkViolet` | 12 | Dark violet |
| `eColorIndexDarkTurquoise` | 13 | Dark turquoise |
| `eColorIndexDarkGrey` | 14 | Dark gray |
| `eColorIndexDarkYellow` | 15 | Dark yellow |
| `eColorIndexWhite` | 16 | White |
| `eColorIndexOtherColors` | 17 | Other colors |
| `eColorIndexPalette` | 18 | Palette |
| `eColorIndexGlobalColorPalette1` | 19 | Global palette 1 |
| `eColorIndexGlobalColorPalette2` | 20 | Global palette 2 |
| `eColorIndexGlobalColorPalette3` | 21 | Global palette 3 |
| `eColorIndexFillEffects` | 22 | Filling effects |

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

oMy2DCurve.Shape.Settings.Filling.Pattern = dd.eFillPatternLeftDiagonal

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColorIndex_IRepPaletteLineColorInt.htm`*
