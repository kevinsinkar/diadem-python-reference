---
title: "IRepColorLegendContentLabelNumInt.Interval"
description: "Specifies that DIAdem REPORT only displays the color symbols of a color legend at every nth legend symbol."
---

# IRepColorLegendContentLabelNumInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for ColorLegendNumbers

Specifies that DIAdem REPORT only displays the color symbols of a color legend at every nth legend symbol.

## Signature

```python
obj.Interval
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
oMyColorLegend.Settings.Numbers.Interval = 2
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

*Source: `ReportApi/properties/Report_property_Interval_IRepColorLegendContentLabelNumInt.htm`*
