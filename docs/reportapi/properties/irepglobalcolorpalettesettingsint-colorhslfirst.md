---
title: "IRepGlobalColorPaletteSettingsInt.ColorHSLFirst"
description: "Specifies the start color of the global color palette in the HSL color model in DIAdem REPORT. Use the RGBToHSL command to convert a color value from the RGB mo"
---

# IRepGlobalColorPaletteSettingsInt.ColorHSLFirst

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColorHSLFirst for GlobalColorPaletteSettings

Specifies the start color of the global color palette in the HSL color model in DIAdem REPORT. Use the RGBToHSL command to convert a color value from the RGB model (red, green, blue) into the HSL model (color, saturation, brightness).

## Signature

```python
obj.ColorHSLFirst
```

## Python example

```python
dd.Report.NewLayout()
oMyGlobalColorPalette = dd.Report.Settings.GlobalColorPalette1
oMyGlobalColorPalette.ColorHSLFirst = dd.RGBtoHSL(dd.RGB(0, 0, 255))
oMyGlobalColorPalette.ColorHSLLast = dd.RGBtoHSL(dd.RGB(255,0,0))
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexGlobalColorPalette1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColorHSLFirst_IRepGlobalColorPaletteSettingsInt.htm`*
