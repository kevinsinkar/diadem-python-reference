---
title: "IRepD2ShapeObjBarsSettingsInt.Palette"
description: "Specifies the properties of the palette which DIAdem REPORT uses for a bars display in a 2D axis system."
---

# IRepD2ShapeObjBarsSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 2DBarsSettings

Specifies the properties of the palette which DIAdem REPORT uses for a bars display in a 2D axis system.

## Signature

```python
return_value = obj.Palette
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[1]"
oMyFilling = oMyShape.Settings.Filling
oMyFilling.Pattern = dd.eFillPatternFilled
oMyFilling.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyShape.Settings.Palette
oMyPalette.ValueType = dd.e2DPaletteValueTypeInputInterval
oMyPalette.BeginValue = 20
oMyPalette.EndValue = 40
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepD2ShapeObjBarsSettingsInt.htm`*
