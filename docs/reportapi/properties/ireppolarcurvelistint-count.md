---
title: "IRepPolarCurveListInt.Count"
description: "Returns the number of curves in a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for PolarCurves

Returns the number of curves in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of curves: " + oMyReportObj.Curves.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepPolarCurveListInt.htm`*
