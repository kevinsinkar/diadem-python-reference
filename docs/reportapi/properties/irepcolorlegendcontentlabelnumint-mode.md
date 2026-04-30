---
title: "IRepColorLegendContentLabelNumInt.Mode"
description: "Specifies how DIAdem REPORT labels the scale of a color legend."
---

# IRepColorLegendContentLabelNumInt.Mode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Mode for ColorLegendNumbers

Specifies how DIAdem REPORT labels the scale of a color legend.

## Signature

```python
obj.Mode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorLegendScaleInterval` | 0 | Interval |
| `eColorLegendScaleSingleValue` | 1 | Single value |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 10
oMyPos.X2 = 60
oMyPos.Y1 = 10
oMyPos.Y2 = 60
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColorLegend = oMy2DAxisSystem.ColorLegend
oMyColorLegend.Visible = True
oMyNumbers = oMyColorLegend.Settings.Numbers
oMyNumbers.Format = "d.dd"
oMyNumbers.Mode = dd.eColorLegendScaleSingleValue
oMyNumbers.ValueMode = dd.eColorLegendScaleValueModeCenter
oMyNumbers.UsePaletteColor = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Mode_IRepColorLegendContentLabelNumInt.htm`*
