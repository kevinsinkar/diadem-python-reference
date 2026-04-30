---
title: "IRepColorLegendInt.Header"
description: "Specifies the properties of the color legend title in an axis system in DIAdem REPORT."
---

# IRepColorLegendInt.Header

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Header for ColorLegend

Specifies the properties of the color legend title in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Header
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
oMyHeader = oMyColorLegend.Header
oMyHeader.Alignment = dd.eLegendHeaderAlignmentRight
oMyHeader.PortionHeaderField = 20
oMyHeader.ShowGrid = True
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

*Source: `ReportApi/properties/Report_property_Header_IRepColorLegendInt.htm`*
