---
title: "IRepColorLegendSettingsInt.Alignment"
description: "Specifies the relative position of the legend label in relation to the symbols in an axis system in DIAdem REPORT."
---

# IRepColorLegendSettingsInt.Alignment

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Alignment for ColorLegendSettings

Specifies the relative position of the legend label in relation to the symbols in an axis system in DIAdem REPORT.

## Signature

```python
obj.Alignment
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendTextAlignmentAutomatic` | 0 | Automatic |
| `eLegendTextAlignmentTop` | 1 | Top |
| `eLegendTextAlignmentBottom` | 2 | Bottom |
| `eLegendTextAlignmentLeft` | 3 | Left |
| `eLegendTextAlignmentRight` | 4 | Right |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColorLegend = oMy2DAxisSystem.ColorLegend
oMyColorLegend.Visible = True
oMyColorLegend.Settings.Alignment = dd.eLegendTextAlignmentRight
oMyNumbers = oMyColorLegend.Settings.Numbers
oMyNumbers.Format = "d.ddde"
oMyNumbers.Mode = dd.eColorLegendScaleSingleValue
oMyNumbers.ValueMode = dd.eColorLegendScaleValueModeCenter
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Alignment_IRepColorLegendSettingsInt.htm`*
