---
title: "IRepColorLegendSettingsInt.SymbolSpace"
description: "Specifies in an axis system in DIAdem REPORT the distance of the surface rectangles of the color legend symbols to each other as a percentage of the rectangular"
---

# IRepColorLegendSettingsInt.SymbolSpace

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SymbolSpace for ColorLegendSettings

Specifies in an axis system in DIAdem REPORT the distance of the surface rectangles of the color legend symbols to each other as a percentage of the rectangular diagonal.

## Signature

```python
obj.SymbolSpace
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 60
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColorLegend = oMy2DAxisSystem.ColorLegend
oMyColorLegend.Visible = True
oMyColorLegend.Settings.SymbolType = dd.eLegendSymbolRectangle
oMyColorLegend.Settings.SymbolSpace = 50
oMyNumbers = oMyColorLegend.Settings.Numbers
oMyNumbers.Format = "d.d"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SymbolSpace_IRepColorLegendSettingsInt.htm`*
