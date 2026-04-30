---
title: "IRepD3PaletteColoredLineListInt.ValueType"
description: "Specifies how DIAdem REPORT assigns the colors from the color palette to the 3D curve in a 3D axis system. DIAdem only includes this setting if the display type"
---

# IRepD3PaletteColoredLineListInt.ValueType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ValueType for 3DPaletteColoredLines

Specifies how DIAdem REPORT assigns the colors from the color palette to the 3D curve in a 3D axis system. DIAdem only includes this setting if the display type is a 3D curve. If the property ValueType has the value e3DPaletteValueTypeWithChnMinMaxRange , the colors are the same as the colors of the y-ranges of the curve. For other values, use the Channel property to specify a color channel, which DIAdem uses for displaying the 3D curve in the palette colors.

## Signature

```python
obj.ValueType
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeLine, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
#oMyShape.DataStructure = e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.ZChannel.Reference = "[3]/[3]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColoredLines = oMyShape.Settings.Palette
oMyColoredLines.ValueType = dd.e3DPaletteValueTypeWithChnMinMaxRange
oMyColoredLines.Channel.Reference = "[3]/[1]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ValueType_IRepD3PaletteColoredLineListInt.htm`*
