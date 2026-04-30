---
title: "IRepColorLegendSettingsInt.PortionSymbolField"
description: "Specifies the size for the color fields of the color legend as a percentage of the legend size in an axis system in DIAdem REPORT."
---

# IRepColorLegendSettingsInt.PortionSymbolField

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PortionSymbolField for ColorLegendSettings

Specifies the size for the color fields of the color legend as a percentage of the legend size in an axis system in DIAdem REPORT.

## Signature

```python
obj.PortionSymbolField
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve.Shape.Settings.Line.Color.ColorIndex=dd.eColorIndexPalette
oMy2DAxisSystem.ColorLegend.Visible = True
oMy2DAxisSystem.ColorLegend.Settings.PortionSymbolField = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PortionSymbolField_IRepColorLegendSettingsInt.htm`*
