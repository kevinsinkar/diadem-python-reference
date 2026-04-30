---
title: "PolarCurves"
description: "Collection of all PolarCurve objects in DIAdem REPORT. Use the PolarCurves collection to access a single curve in a polar axis system."
---

# PolarCurves

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: PolarCurves

Collection of all PolarCurve objects in DIAdem REPORT. Use the PolarCurves collection to access a single curve in a polar axis system.

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
<p><a href="../../properties/ireppolarcurvelistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireppolarcurvelistint-add/">Add</a> | <a href="../../methods/ireppolarcurvelistint-changeshape/">ChangeShape</a> | <a href="../../methods/ireppolarcurvelistint-copy/">Copy</a> | <a href="../../methods/ireppolarcurvelistint-exists/">Exists</a> | <a href="../../methods/ireppolarcurvelistint-item/">Item</a> | <a href="../../methods/ireppolarcurvelistint-move/">Move</a> | <a href="../../methods/ireppolarcurvelistint-remove/">Remove</a> | <a href="../../methods/ireppolarcurvelistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ireppolarint/">PolarSystem</a>.<a href="../../properties/ireppolarint-curvespolar/">CurvesPolar</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarCurveListInt.htm`*
