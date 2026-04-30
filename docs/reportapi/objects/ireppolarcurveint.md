---
title: "IRepPolarCurveInt"
description: "The PolarCurve object provides a polar axis system curve in DIAdem REPORT."
---

# IRepPolarCurveInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarCurve

The PolarCurve object provides a polar axis system curve in DIAdem REPORT.

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        oMySubObjects = oMyReportObj.CurvesPolar
        for oMySubObj in oMySubObjects:
            sOutput = sOutput + "Curve shape: " + oMySubObj.ShapeType + "\t" + "Curve name: " + oMySubObj.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarcurveint-enable/">Enable</a> | <a href="../../properties/ireppolarcurveint-index/">Index</a> | <a href="../../properties/ireppolarcurveint-legendicontype/">LegendIconType</a> | <a href="../../properties/ireppolarcurveint-name/">Name</a> | <a href="../../properties/ireppolarcurveint-relatedlegendtext/">RelatedLegendText</a> | <a href="../../properties/ireppolarcurveint-shape/">Shape</a> | <a href="../../properties/ireppolarcurveint-shapetype/">ShapeType</a> | <a href="../../properties/ireppolarcurveint-tagstored/">TagStored</a> | <a href="../../properties/ireppolarcurveint-tagtemporary/">TagTemporary</a> | <a href="../../properties/ireppolarcurveint-usecurveexpansion/">UseCurveExpansion</a> | <a href="../../properties/ireppolarcurveint-visibleinlegend/">VisibleInLegend</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireppolarcurveint-isexpanded/">IsExpanded</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../methods/ireppolarcurvelistint-add/">Add</a> | <a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../methods/ireppolarcurvelistint-changeshape/">ChangeShape</a> | <a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../methods/ireppolarcurvelistint-copy/">Copy</a> | <a href="../../collections/polarcurves/">PolarCurves</a>.<a href="../../methods/ireppolarcurvelistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarCurveInt.htm`*
