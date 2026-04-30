---
title: "IRepSpiderCurveInt.Index"
description: "Returns the index of a curve in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for SpiderCurve

Returns the index of a curve in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Index
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType ==dd.eReportObjectSpider :
        oMySubObjects = oMyReportObj.CurvesSpider
        for i in range( 1, oMySubObjects.Count+1):
            sOutput = sOutput + "Curve Index: " + oMySubObjects.Item(i).Index + "\t" + "Curve name: " + oMySubObjects.Item(i).Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepSpiderCurveInt.htm`*
