---
title: "IRepD2AxisXScalingInt.SynchronizationID"
description: "Specifies the unique names of the synchronization groups assigned to an x-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXScalingInt.SynchronizationID

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SynchronizationID for 2DAxisXScaling

Specifies the unique names of the synchronization groups assigned to an x-axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.SynchronizationID
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

*Source: `ReportApi/properties/Report_property_SynchronizationID_IRepD2AxisXScalingInt.htm`*
