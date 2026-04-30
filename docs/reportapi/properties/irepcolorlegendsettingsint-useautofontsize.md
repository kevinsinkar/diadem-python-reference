---
title: "IRepColorLegendSettingsInt.UseAutoFontSize"
description: "Specifies whether DIAdem REPORT determines the font size of the color legend label automatically in an axis system."
---

# IRepColorLegendSettingsInt.UseAutoFontSize

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseAutoFontSize for ColorLegendSettings

Specifies whether DIAdem REPORT determines the font size of the color legend label automatically in an axis system.

## Signature

```python
obj.UseAutoFontSize
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 60
oMyPosition.Y1 = 10
oMyPosition.Y2 = 60
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColorLegend = oMy2DAxisSystem.ColorLegend
oMyColorLegend.Visible = True
oMyColorLegend.Settings.UseAutoFontSize = True
oMyNumbers = oMyColorLegend.Settings.Numbers
oMyNumbers.Format = "d.ddde"
oMyNumbers.Mode = dd.eColorLegendScaleSingleValue
oMyNumbers.ValueMode = dd.eColorLegendScaleValueModeCenter
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseAutoFontSize_IRepColorLegendSettingsInt.htm`*
