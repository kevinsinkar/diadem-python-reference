---
title: "IRepD2CurveListInt.Count"
description: "Returns the number of curves in a 2D axis system in DIAdem REPORT."
---

# IRepD2CurveListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 2DCurves

Returns the number of curves in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of curves: " + oMyReportObj.Curves2D.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepD2CurveListInt.htm`*
