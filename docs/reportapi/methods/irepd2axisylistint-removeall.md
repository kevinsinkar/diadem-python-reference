---
title: "IRepD2AxisYListInt.RemoveAll"
description: "Deletes all additional y-axes in a 2D axis system in DIAdem REPORT. You cannot delete the first y-axis."
---

# IRepD2AxisYListInt.RemoveAll

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: RemoveAll for 2DAxisYAxisList

Deletes all additional y-axes in a 2D axis system in DIAdem REPORT. You cannot delete the first y-axis.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMyReportObj.YAxisList.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_RemoveAll_IRepD2AxisYListInt.htm`*
