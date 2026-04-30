---
title: "IRepD2CurveInt"
description: "The 2DCurve object provides a curve in a 2D axis system in DIAdem REPORT."
---

# IRepD2CurveInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DCurve

The 2DCurve object provides a curve in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2curveint-enable/">Enable</a> | <a href="../../properties/irepd2curveint-index/">Index</a> | <a href="../../properties/irepd2curveint-legendicontype/">LegendIconType</a> | <a href="../../properties/irepd2curveint-name/">Name</a> | <a href="#" data-unresolved="1">OnCurveTransformation</a> | <a href="../../properties/irepd2curveint-relatedlegendtext/">RelatedLegendText</a> | <a href="../../properties/irepd2curveint-shape/">Shape</a> | <a href="../../properties/irepd2curveint-shapetype/">ShapeType</a> | <a href="../../properties/irepd2curveint-tagstored/">TagStored</a> | <a href="../../properties/irepd2curveint-tagtemporary/">TagTemporary</a> | <a href="../../properties/irepd2curveint-visibleinlegend/">VisibleInLegend</a> | <a href="../../properties/irepd2curveint-yaxisreference/">YAxisReference</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd2curveint-findnearestvalue/">FindNearestValue</a> | <a href="../../methods/irepd2curveint-isexpanded/">IsExpanded</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../methods/irepd2curvelistint-add/">Add</a> | <a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../methods/irepd2curvelistint-changeshape/">ChangeShape</a> | <a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../methods/irepd2curvelistint-copy/">Copy</a> | <a href="../../collections/2dcurves/">2DCurves</a>.<a href="../../methods/irepd2curvelistint-item/">Item</a> | <a href="../irepd2curvetransformingcontextint/">D2CurveTransformingContext</a>.<a href="../../properties/irepd2curvetransformingcontextint-curve/">Curve</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2CurveInt.htm`*
