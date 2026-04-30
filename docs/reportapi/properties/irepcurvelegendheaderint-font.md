---
title: "IRepCurveLegendHeaderInt.Font"
description: "Specifies the font of the curve legend heading in an axis system in DIAdem REPORT."
---

# IRepCurveLegendHeaderInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for CurveLegendHeader

Specifies the font of the curve legend heading in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyAnchor = oMyLegend.Position.Anchor
oMyAnchor.PageRelatedX = 10
oMyAnchor.PageRelatedY = 20
oMyLegend.Columns(1).Title = "Legend Title"
oMyLegendHeader = oMyLegend.Header
oMyLegendHeader.ShowGrid = True
oMyLegendHeader.PortionHeaderField = 5
oMyLegendHeader.Font.Name = "Times Roman"()
oMyLegendHeader.Font.Bold = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepCurveLegendHeaderInt.htm`*
