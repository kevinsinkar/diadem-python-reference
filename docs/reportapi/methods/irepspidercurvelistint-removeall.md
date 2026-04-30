---
title: "IRepSpiderCurveListInt.RemoveAll"
description: "Deletes all curves of a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveListInt.RemoveAll

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: RemoveAll for SpiderCurves

Deletes all curves of a spider axis system in DIAdem REPORT.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectSpider :
        oMyReportObj.CurvesSpider.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_RemoveAll_IRepSpiderCurveListInt.htm`*
