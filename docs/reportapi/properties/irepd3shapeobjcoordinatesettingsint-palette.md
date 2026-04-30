---
title: "IRepD3ShapeObjCoordinateSettingsInt.Palette"
description: "Specifies the properties of the palette which DIAdem REPORT uses for a coordinate display in a 3D axis system."
---

# IRepD3ShapeObjCoordinateSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 3DCoordinateSettings

Specifies the properties of the palette which DIAdem REPORT uses for a coordinate display in a 3D axis system.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMy3DCoord = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCoordinate, "MyNew3DCoordinate")
oMyCoordShape = oMy3DCoord.Shape
oMyCoordShape.BoundingType = dd.eCoordinateChannelBounded
oMyCoordShape.DataStructure = dd.e3DDataStructureTriplet
oMyCoordShape.BoundingPosition = dd.e3DCoordinateBoundingInterpolation
oMyCoordShape.BoundingXChannel.Reference = "[2]/[1]"
oMyCoordShape.BoundingYChannel.Reference = "[2]/[2]"
oMyCoordShape.BoundingZChannel.Reference = "[2]/[3]"
oMyCoordShape.XCoordinate.Reference = 0.7
oMyCoordShape.YCoordinate.Reference = 0.5
oMyCoordShape.Extensions.CoordinateComment.Visible = True
oMyCoordSettings = oMyCoordShape.Settings
oMyCoordSettings.MarkerLine.Color.ColorIndex = dd.eColorIndexPalette
oMyCoordSettings.Size = 3
oMyPaletteColoredLines = oMyCoordShape.Settings.Palette
oMyPaletteColoredLines.Count = 10
for i in range( 1, oMyPaletteColoredLines.Count+1):
    oMyPaletteColoredLines(i).Color.SetPredefinedColor(i)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepD3ShapeObjCoordinateSettingsInt.htm`*
