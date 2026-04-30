---
title: "IRepLegendPositionAnchorInt"
description: "The LegendPositionAnchor object provides the properties of an anchor point of a curve legend and a color legend in DIAdem REPORT."
---

# IRepLegendPositionAnchorInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: LegendPositionAnchor

The LegendPositionAnchor object provides the properties of an anchor point of a curve legend and a color legend in DIAdem REPORT.

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
<p><a href="../../properties/ireplegendpositionanchorint-pagerelatedx/">PageRelatedX</a> | <a href="../../properties/ireplegendpositionanchorint-pagerelatedy/">PageRelatedY</a> | <a href="../../properties/ireplegendpositionanchorint-systemrelatedx/">SystemRelatedX</a> | <a href="../../properties/ireplegendpositionanchorint-systemrelatedy/">SystemRelatedY</a> | <a href="../../properties/ireplegendpositionanchorint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireplegendpositionint/">LegendPosition</a>.<a href="../../properties/ireplegendpositionint-anchor/">Anchor</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLegendPositionAnchorInt.htm`*
