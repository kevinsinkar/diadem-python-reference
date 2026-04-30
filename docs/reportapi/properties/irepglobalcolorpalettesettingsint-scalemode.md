---
title: "IRepGlobalColorPaletteSettingsInt.ScaleMode"
description: "Specifies how to assign a value range to a global color palette in DIAdem REPORT."
---

# IRepGlobalColorPaletteSettingsInt.ScaleMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ScaleMode for GlobalColorPaletteSettings

Specifies how to assign a value range to a global color palette in DIAdem REPORT.

## Signature

```python
obj.ScaleMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eGlobalColorPaletteScaleAxisScalingRange` | 0 | Axis scaling range |
| `eGlobalColorPaletteScaleDistanceOfAxisTicks` | 1 | Interval between the ticks |
| `eGlobalColorPaletteScaleInputValueRange` | 2 | Enter value range |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyGlobalPalette = dd.Report.Settings.GlobalColorPalette1
oMyGlobalPalette.ScaleMode = dd.eGlobalColorPaletteScaleDistanceOfAxisTicks
oMyGlobalPalette.ScaleValueBegin = 0.2
oMyGlobalPalette.ScaleValueEnd = 0.6

oMyGlobalColorPaletteLine = dd.Report.Settings.GlobalColorPalette1.LineStyle
oMyGlobalColorPaletteLine.Width = dd.eLineWidth0100
oMyGlobalColorPaletteLine.LineType = dd.eLineTypeDashed1
oMyGlobalColorPaletteLine.Interval = 5

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
dd.Report.refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ScaleMode_IRepGlobalColorPaletteSettingsInt.htm`*
