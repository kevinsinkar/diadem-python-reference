---
title: "IRepPaletteLineInt.Color"
description: "Specifies the colors of the color palette in a 2D axis system in DIAdem REPORT."
---

# IRepPaletteLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for PaletteLine

Specifies the colors of the color palette in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepPaletteLineInt.htm`*
