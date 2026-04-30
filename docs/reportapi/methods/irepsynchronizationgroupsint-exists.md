---
title: "IRepSynchronizationGroupsInt.Exists"
description: "Checks whether a synchronization group exists in the list of synchronization groups in DIAdem REPORT."
---

# IRepSynchronizationGroupsInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for SynchronizationGroups

Checks whether a synchronization group exists in the list of synchronization groups in DIAdem REPORT.

## Signature

```python
bExists = Object.Exists(ID)
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

*Source: `ReportApi/methods/Report_method_Exists_IRepSynchronizationGroupsInt.htm`*
