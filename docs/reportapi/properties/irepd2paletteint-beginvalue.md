---
title: "IRepD2PaletteInt.BeginValue"
description: "Specifies the lower limit of the y-range in which DIAdem REPORT displays a curve with a color palette. The EndValue property specifies the upper limit of this y"
---

# IRepD2PaletteInt.BeginValue

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BeginValue for 2DPalette

Specifies the lower limit of the y-range in which DIAdem REPORT displays a curve with a color palette. The EndValue property specifies the upper limit of this y-range.

## Signature

```python
obj.BeginValue
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyCurve.Shape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyCurve.Shape.Settings.Palette.ValueType = dd.e2DPaletteValueTypeInputInterval
oMyCurve.Shape.Settings.Palette.BeginValue = 5
oMyCurve.Shape.Settings.Palette.EndValue = 30
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BeginValue_IRepD2PaletteInt.htm`*
