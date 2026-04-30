---
title: "IRepD3CurveListInt.Remove"
description: "Deletes a curve from a 3D axis system in DIAdem REPORT."
---

# IRepD3CurveListInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for 3DCurves

Deletes a curve from a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        iCurveCount = oMyReportObj.Curves3D.Count
        if iCurveCount > 1 :
            oMyReportObj.Curves3D.Remove(iCurveCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepD3CurveListInt.htm`*
