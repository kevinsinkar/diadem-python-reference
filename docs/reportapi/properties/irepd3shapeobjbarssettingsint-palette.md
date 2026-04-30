---
title: "IRepD3ShapeObjBarsSettingsInt.Palette"
description: "Specifies the properties of the palette which DIAdem REPORT uses for a bars display in a 3D axis system."
---

# IRepD3ShapeObjBarsSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 3DBarsSettings

Specifies the properties of the palette which DIAdem REPORT uses for a bars display in a 3D axis system.

## Signature

```python
return_value = obj.Palette
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeBars, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMy3DCurve.Shape.Settings
oMySettings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyPaletteColoredLines = oMySettings.Palette
oMyPaletteColoredLines.Count = 10
for oMyColoredLine in oMyPaletteColoredLines:
    oMyColoredLine.Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepD3ShapeObjBarsSettingsInt.htm`*
