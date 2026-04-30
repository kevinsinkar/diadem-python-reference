---
title: "IRepColorLegendHeaderInt.Alignment"
description: "Specifies the relative position of the text field within a color legend in an axis system in DIAdem REPORT."
---

# IRepColorLegendHeaderInt.Alignment

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Alignment for ColorLegendHeader

Specifies the relative position of the text field within a color legend in an axis system in DIAdem REPORT.

## Signature

```python
obj.Alignment
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendHeaderAlignmentLeft` | 0 | Left |
| `eLegendHeaderAlignmentRight` | 1 | Right |
| `eLegendHeaderAlignmentTop` | 2 | Top |
| `eLegendHeaderAlignmentBottom` | 3 | Bottom |

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
oMyLegendHeader.Alignment = dd.eLegendHeaderAlignmentTop
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Alignment_IRepColorLegendHeaderInt.htm`*
