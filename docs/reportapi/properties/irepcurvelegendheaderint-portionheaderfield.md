---
title: "IRepCurveLegendHeaderInt.PortionHeaderField"
description: "Specifies the size of the field for the general header of the curve legend as a percentage of the page in an axis system in DIAdem REPORT."
---

# IRepCurveLegendHeaderInt.PortionHeaderField

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PortionHeaderField for CurveLegendHeader

Specifies the size of the field for the general header of the curve legend as a percentage of the page in an axis system in DIAdem REPORT.

## Signature

```python
obj.PortionHeaderField
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
oMyLegendHeader.PortionHeaderField = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PortionHeaderField_IRepCurveLegendHeaderInt.htm`*
