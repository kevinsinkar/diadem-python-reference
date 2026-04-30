---
title: "IRepD2AxisYListInt.Count"
description: "Returns the number of y-axes in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 2DAxisYAxisList

Returns the number of y-axes in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of axes: " + oMyReportObj.YAxisList.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepD2AxisYListInt.htm`*
