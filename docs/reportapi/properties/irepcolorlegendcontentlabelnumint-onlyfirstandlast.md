---
title: "IRepColorLegendContentLabelNumInt.OnlyFirstAndLast"
description: "Specifies whether DIAdem REPORT only labels the first and last value of a color legend in an axis system."
---

# IRepColorLegendContentLabelNumInt.OnlyFirstAndLast

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OnlyFirstAndLast for ColorLegendNumbers

Specifies whether DIAdem REPORT only labels the first and last value of a color legend in an axis system.

## Signature

```python
obj.OnlyFirstAndLast
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 60
oMyCurve = oMy2DAxisSystem.Curves2D.Add(e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = eColorIndexPalette
oMyColorLegend = oMy2DAxisSystem.ColorLegend
oMyColorLegend.Visible = True
oMyLegendNumbers = oMyColorLegend.Settings.Numbers
oMyLegendNumbers.Mode = eColorLegendScaleSingleValue
oMyLegendNumbers.ValueMode = eColorLegendScaleValueModeBoundary
oMyLegendNumbers.OnlyFirstAndLast = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OnlyFirstAndLast_IRepColorLegendContentLabelNumInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
