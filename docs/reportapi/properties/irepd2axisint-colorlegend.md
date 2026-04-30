---
title: "IRepD2AxisInt.ColorLegend"
description: "Specifies the color legend of a 2D axis system in DIAdem REPORT. Select Palette as the curve color in order to enable the color legend."
---

# IRepD2AxisInt.ColorLegend

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColorLegend for 2DAxisSystem

Specifies the color legend of a 2D axis system in DIAdem REPORT. Select Palette as the curve color in order to enable the color legend.

## Signature

```python
return_value = obj.ColorLegend
```

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
oMy2DAxisSystem.ColorLegend.Visible = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColorLegend_IRepD2AxisInt.htm`*
