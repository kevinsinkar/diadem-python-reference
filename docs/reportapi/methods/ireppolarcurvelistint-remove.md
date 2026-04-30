---
title: "IRepPolarCurveListInt.Remove"
description: "Deletes a curve from a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveListInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for PolarCurves

Deletes a curve from a polar axis system in DIAdem REPORT.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        oMyReportObj.CurvesPolar.Remove(1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepPolarCurveListInt.htm`*
