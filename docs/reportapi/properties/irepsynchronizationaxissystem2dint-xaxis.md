---
title: "IRepSynchronizationAxisSystem2DInt.XAxis"
description: "Specifies the list of the synchronization groups of the x-axes of 2D axis systems in DIAdem REPORT."
---

# IRepSynchronizationAxisSystem2DInt.XAxis

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XAxis for SynchronizationAxisSystem2D

Specifies the list of the synchronization groups of the x-axes of 2D axis systems in DIAdem REPORT.

## Signature

```python
return_value = obj.XAxis
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

*Source: `ReportApi/properties/Report_property_XAxis_IRepSynchronizationAxisSystem2DInt.htm`*
