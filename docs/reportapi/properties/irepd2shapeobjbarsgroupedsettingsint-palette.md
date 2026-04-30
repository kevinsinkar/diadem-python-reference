---
title: "IRepD2ShapeObjBarsGroupedSettingsInt.Palette"
description: "Specifies the palette properties of a bar in the Grouped bars display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjBarsGroupedSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 2DGroupedBarsSettings

Specifies the palette properties of a bar in the Grouped bars display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Palette
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

oMyPaletteSettings = oMy2DCurve.Shape.Settings.Palette
oMyPaletteSettings.Colors(1).ColorIndex = dd.eColorIndexViolet
oMyPaletteSettings.Colors(2).ColorIndex = dd.eColorIndexYellow

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepD2ShapeObjBarsGroupedSettingsInt.htm`*
