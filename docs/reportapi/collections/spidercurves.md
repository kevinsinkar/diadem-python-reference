---
title: "SpiderCurves"
description: "Collection of all SpiderCurve objects in DIAdem REPORT. Use the SpiderCurves collection to access a single curve in a spider axis system."
---

# SpiderCurves

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: SpiderCurves

Collection of all SpiderCurve objects in DIAdem REPORT. Use the SpiderCurves collection to access a single curve in a spider axis system.

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectSpider :
        oMySubObjects = oMyReportObj.CurvesSpider
        for oMySubObj in oMySubObjects:
            sOutput = sOutput + "Curve shape: " + oMySubObj.ShapeType + "\t" + "Curve name: " + oMySubObj.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/irepspidercurvelistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepspidercurvelistint-add/">Add</a> | <a href="../../methods/irepspidercurvelistint-changeshape/">ChangeShape</a> | <a href="../../methods/irepspidercurvelistint-copy/">Copy</a> | <a href="../../methods/irepspidercurvelistint-exists/">Exists</a> | <a href="../../methods/irepspidercurvelistint-item/">Item</a> | <a href="../../methods/irepspidercurvelistint-move/">Move</a> | <a href="../../methods/irepspidercurvelistint-remove/">Remove</a> | <a href="../../methods/irepspidercurvelistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepspiderint/">Spider</a>.<a href="../../properties/irepspiderint-curvesspider/">CurvesSpider</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderCurveListInt.htm`*
