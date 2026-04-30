---
title: "IRepSpiderCurveListInt.Remove"
description: "Deletes a curve from a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveListInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for SpiderCurves

Deletes a curve from a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectSpider :
        oMyReportObj.CurvesSpider.Remove(1)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepSpiderCurveListInt.htm`*
