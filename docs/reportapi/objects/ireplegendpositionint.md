---
title: "IRepLegendPositionInt"
description: "The LegendPosition object provides the position properties of a curve legend and a color legend in DIAdem REPORT."
---

# IRepLegendPositionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: LegendPosition

The LegendPosition object provides the position properties of a curve legend and a color legend in DIAdem REPORT.

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
oMyAnchor.PageRelatedY = 10
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireplegendpositionint-anchor/">Anchor</a> | <a href="../../properties/ireplegendpositionint-elementheight/">ElementHeight</a> | <a href="../../properties/ireplegendpositionint-elementwidth/">ElementWidth</a> | <a href="../../properties/ireplegendpositionint-entireheight/">EntireHeight</a> | <a href="../../properties/ireplegendpositionint-entirewidth/">EntireWidth</a> | <a href="../../properties/ireplegendpositionint-interactivemovemode/">InteractiveMoveMode</a> | <a href="../../properties/ireplegendpositionint-relativeposition/">RelativePosition</a> | <a href="../../properties/ireplegendpositionint-sizemode/">SizeMode</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcolorlegendint/">ColorLegend</a>.<a href="../../properties/irepcolorlegendint-position/">Position</a> | <a href="../irepcurvelegendint/">CurveLegend</a>.<a href="../../properties/irepcurvelegendint-position/">Position</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLegendPositionInt.htm`*
