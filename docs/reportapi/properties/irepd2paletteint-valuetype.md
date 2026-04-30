---
title: "IRepD2PaletteInt.ValueType"
description: "Specifies how DIAdem REPORT assigns the colors from the color palette to the curve in a 2D axis system. If the property ValueType has the value e2DPaletteValueT"
---

# IRepD2PaletteInt.ValueType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ValueType for 2DPalette

Specifies how DIAdem REPORT assigns the colors from the color palette to the curve in a 2D axis system. If the property ValueType has the value e2DPaletteValueTypeAxisScalingRange , e2DPaletteValueTypeDistanceOfAxisTicks , or e2DPaletteValueTypeInputInterval , the colors are the same as the colors of the y-ranges of the curve. For other values, use the Channel property to specify a color channel, which DIAdem uses for displaying the curve in the palette colors.

## Signature

```python
obj.ValueType
```

## Python example

```python
dd.Report.NewLayout()
oMyReportObj = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMyReportObj.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyReportObj.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
iChannelMax = dd.Data.Root.ChannelGroups(1).Channels(2).Properties("maximum").Value
iChannelMin = dd.Data.Root.ChannelGroups(1).Channels(2).Properties("minimum").Value
oMyLine = oMyShape.Settings.Line
oMyLine.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyShape.Settings.Palette
oMyPalette.ValueType = dd.e2DPaletteValueTypeDistanceOfAxisTicks
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ValueType_IRepD2PaletteInt.htm`*
