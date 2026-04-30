---
title: "IRepPolarCurveListInt.RemoveAll"
description: "Deletes all curves in a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveListInt.RemoveAll

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: RemoveAll for PolarCurves

Deletes all curves in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        oMyReportObj.CurvesPolar.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_RemoveAll_IRepPolarCurveListInt.htm`*
