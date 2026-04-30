---
title: "IRepSpiderCurveInt"
description: "The SpiderCurve object provides a category in a spider axis system curve in DIAdem REPORT."
---

# IRepSpiderCurveInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderCurve

The SpiderCurve object provides a category in a spider axis system curve in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"
oMyCurve.Enable = True

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepspidercurveint-enable/">Enable</a> | <a href="../../properties/irepspidercurveint-index/">Index</a> | <a href="../../properties/irepspidercurveint-legendicontype/">LegendIconType</a> | <a href="../../properties/irepspidercurveint-name/">Name</a> | <a href="../../properties/irepspidercurveint-relatedlegendtext/">RelatedLegendText</a> | <a href="../../properties/irepspidercurveint-shape/">Shape</a> | <a href="../../properties/irepspidercurveint-shapetype/">ShapeType</a> | <a href="../../properties/irepspidercurveint-tagstored/">TagStored</a> | <a href="../../properties/irepspidercurveint-tagtemporary/">TagTemporary</a> | <a href="../../properties/irepspidercurveint-visibleinlegend/">VisibleInLegend</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepspidercurveint-isexpanded/">IsExpanded</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/spidercurves/">SpiderCurves</a>.<a href="../../methods/irepspidercurvelistint-add/">Add</a> | <a href="../../collections/spidercurves/">SpiderCurves</a>.<a href="../../methods/irepspidercurvelistint-changeshape/">ChangeShape</a> | <a href="../../collections/spidercurves/">SpiderCurves</a>.<a href="../../methods/irepspidercurvelistint-copy/">Copy</a> | <a href="../../collections/spidercurves/">SpiderCurves</a>.<a href="../../methods/irepspidercurvelistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderCurveInt.htm`*
