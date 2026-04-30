---
title: "IRepColorLegendHeaderInt.Font"
description: "Specifies the font of the color legend title in an axis system in DIAdem REPORT."
---

# IRepColorLegendHeaderInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for ColorLegendHeader

Specifies the font of the color legend title in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 70
oMyPosition.Y1 = 10
oMyPosition.Y2 = 70
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyCurve.Shape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyLegend = oMy2DAxisSystem.ColorLegend
oMyLegend.Visible = True
oMyAnchor = oMyLegend.Position.Anchor
oMyAnchor.PageRelatedX = 70
oMyAnchor.PageRelatedY = 10
oMyLegendHeader = oMyLegend.Header
oMyLegendHeader.ShowGrid = True
oMyLegendHeader.PortionHeaderField = 5
oMyLegendHeader.Title = "Legend Title"
oMyLegendHeader.Font.Name = "Times Roman"()
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepColorLegendHeaderInt.htm`*
