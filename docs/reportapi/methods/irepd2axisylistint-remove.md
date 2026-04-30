---
title: "IRepD2AxisYListInt.Remove"
description: "Deletes an additional y-axis from a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYListInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for 2DAxisYAxisList

Deletes an additional y-axis from a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        iYAxisCount = oMyReportObj.YAxisList.Count
        if iYAxisCount > 1 :
            oMyReportObj.YAxisList.Remove(iYAxisCount)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepD2AxisYListInt.htm`*
