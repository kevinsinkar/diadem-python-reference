---
title: "IRepSynchronizationGroupsInt.Add"
description: "Adds a synchronization group to the list of synchronization groups in DIAdem REPORT."
---

# IRepSynchronizationGroupsInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for SynchronizationGroups

Adds a synchronization group to the list of synchronization groups in DIAdem REPORT.

## Signature

```python
return_value = obj.Add(ID)
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

*Source: `ReportApi/methods/Report_method_Add_IRepSynchronizationGroupsInt.htm`*
