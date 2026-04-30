---
title: "IRepColorLegendSettingsInt.SymbolType"
description: "Specifies whether DIAdem REPORT displays the symbols of the color legend of an axis system as rectangles or as lines."
---

# IRepColorLegendSettingsInt.SymbolType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SymbolType for ColorLegendSettings

Specifies whether DIAdem REPORT displays the symbols of the color legend of an axis system as rectangles or as lines.

## Signature

```python
obj.SymbolType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendSymbolRectangle` | 0 | Rectangle |
| `eLegendSymbolLine` | 1 | Line |

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
oMyColorLegend.Settings.SymbolType = dd.eLegendSymbolLine
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

*Source: `ReportApi/properties/Report_property_SymbolType_IRepColorLegendSettingsInt.htm`*
