---
title: "IRepD2CurveListInt.Remove"
description: "Deletes a curve from a 2D axis system in DIAdem REPORT."
---

# IRepD2CurveListInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for 2DCurves

Deletes a curve from a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        iCurveCount = oMyReportObj.Curves2D.Count
        if iCurveCount > 1 :
            oMyReportObj.Curves2D.Remove(iCurveCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepD2CurveListInt.htm`*
