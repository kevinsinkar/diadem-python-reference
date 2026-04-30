---
title: "IRepD3PaletteColoredLineListInt.Channel"
description: "Specifies the channel with the values that DIAdem uses to display the 3D curve in the colors of the palette. DIAdem only includes this color channel if the prop"
---

# IRepD3PaletteColoredLineListInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for 3DPaletteColoredLines

Specifies the channel with the values that DIAdem uses to display the 3D curve in the colors of the palette. DIAdem only includes this color channel if the property ValueType has the value e2DPaletteValueTypeWithChnMinMaxRange and if the display type is a 3D curve.

## Signature

```python
return_value = obj.Channel
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

*Source: `ReportApi/properties/Report_property_Channel_IRepD3PaletteColoredLineListInt.htm`*
