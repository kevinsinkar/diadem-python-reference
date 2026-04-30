---
title: "IRepSynchronizationAxisSystem2DInt.YAxis"
description: "Specifies the list of synchronization groups of the y-axes of 2D axis system in DIAdem REPORT."
---

# IRepSynchronizationAxisSystem2DInt.YAxis

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XAxis for SynchronizationAxisSystem2D

Specifies the list of synchronization groups of the y-axes of 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.YAxis
```

## Python example

```python
oMyXSync = dd.Report.Settings.Synchronization.AxisSystem2D.XAxis
if not oMyXSync.Exists("YAxis Group1") :
    oMyXSync.Add("YAxis Group1")
oMyReportObjs = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjs:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMyReportObj.YAxis.Scaling.SynchronizationID = "YAxis Group1"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YAxis_IRepSynchronizationAxisSystem2DInt.htm`*
