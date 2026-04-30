---
title: "IRepCurveLegendHeaderInt"
description: "The ColorLegendHeader object provides the title properties of a curve legend in DIAdem REPORT."
---

# IRepCurveLegendHeaderInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CurveLegendHeader

The ColorLegendHeader object provides the title properties of a curve legend in DIAdem REPORT.

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
oMyAnchor.PageRelatedX = 70
oMyAnchor.PageRelatedY = 15
oMyLegend.Columns(1).Title = "Legend Title"
oMyLegendHeader = oMyLegend.Header
oMyLegendHeader.ShowGrid = True
oMyLegendHeader.PortionHeaderField = 5
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcurvelegendheaderint-alignment/">Alignment</a> | <a href="../../properties/irepcurvelegendheaderint-angle/">Angle</a> | <a href="../../properties/irepcurvelegendheaderint-font/">Font</a> | <a href="../../properties/irepcurvelegendheaderint-portionheaderfield/">PortionHeaderField</a> | <a href="../../properties/irepcurvelegendheaderint-showgrid/">ShowGrid</a> | <a href="../../properties/irepcurvelegendheaderint-useautofontsize/">UseAutoFontSize</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcurvelegendint/">CurveLegend</a>.<a href="../../properties/irepcurvelegendint-header/">Header</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCurveLegendHeaderInt.htm`*
