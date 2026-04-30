---
title: "IRepSynchronizationInt.AxisSystem2D"
description: "Specifies the axis system of a synchronization group in DIAdem REPORT."
---

# IRepSynchronizationInt.AxisSystem2D

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AxisSystem2D for Synchronization

Specifies the axis system of a synchronization group in DIAdem REPORT.

## Signature

```python
return_value = obj.AxisSystem2D
```

## Python example

```python
oMyXSync = dd.Report.Settings.Synchronization.AxisSystem2D.XAxis
if not oMyXSync.Exists("XAxis Group1") :
    oMyXSync.Add("XAxis Group1")
oMyReportObjs = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjs:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMyReportObj.XAxis.Scaling.SynchronizationID = "XAxis Group1"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AxisSystem2D_IRepSynchronizationInt.htm`*
