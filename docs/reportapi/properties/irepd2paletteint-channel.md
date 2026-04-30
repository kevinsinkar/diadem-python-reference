---
title: "IRepD2PaletteInt.Channel"
description: "Specifies the channel with the values that DIAdem uses to display the curve in the colors of the palette. DIAdem only includes this color channel if the propert"
---

# IRepD2PaletteInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for 2DPalette

Specifies the channel with the values that DIAdem uses to display the curve in the colors of the palette. DIAdem only includes this color channel if the property ValueType has the value e2DPaletteValueTypeWithChnMinMaxRange , e2DPaletteValueTypeWithChnInputInterval or e2DPaletteValueTypeWithChnInputValueRange .

## Signature

```python
return_value = obj.Channel
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
oMyLine = oMyShape.Settings.Line
oMyLine.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyShape.Settings.Palette
oMyPalette.ValueType = dd.e2DPaletteValueTypeWithChnMinMaxRange
oMyPalette.Channel.Reference = "[1]/[3]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepD2PaletteInt.htm`*
