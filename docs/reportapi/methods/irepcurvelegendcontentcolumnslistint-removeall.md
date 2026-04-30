---
title: "IRepCurvelegendContentColumnsListInt.RemoveAll"
description: "Deletes all columns of a curve legend except the first column DIAdem REPORT."
---

# IRepCurvelegendContentColumnsListInt.RemoveAll

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: RemoveAll for CurveLegendColumns

Deletes all columns of a curve legend except the first column DIAdem REPORT.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMyReportObj.CurveLegend.Columns.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_RemoveAll_IRepCurvelegendContentColumnsListInt.htm`*
