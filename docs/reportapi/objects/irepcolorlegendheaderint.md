---
title: "IRepColorLegendHeaderInt"
description: "The ColorLegendHeader object provides the title properties of a color legend in DIAdem REPORT."
---

# IRepColorLegendHeaderInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ColorLegendHeader

The ColorLegendHeader object provides the title properties of a color legend in DIAdem REPORT.

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
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcolorlegendheaderint-alignment/">Alignment</a> | <a href="../../properties/irepcolorlegendheaderint-angle/">Angle</a> | <a href="../../properties/irepcolorlegendheaderint-font/">Font</a> | <a href="../../properties/irepcolorlegendheaderint-portionheaderfield/">PortionHeaderField</a> | <a href="../../properties/irepcolorlegendheaderint-showgrid/">ShowGrid</a> | <a href="../../properties/irepcolorlegendheaderint-title/">Title</a> | <a href="../../properties/irepcolorlegendheaderint-useautofontsize/">UseAutoFontSize</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcolorlegendint/">ColorLegend</a>.<a href="../../properties/irepcolorlegendint-header/">Header</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepColorLegendHeaderInt.htm`*
