---
title: "IRepSynchronizationGroupInt"
description: "The SynchronizationGroup object provides a synchronization group. DIAdem automatically adjusts the scaling of all axes that belong to the same synchronization g"
---

# IRepSynchronizationGroupInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SynchronizationGroup

The SynchronizationGroup object provides a synchronization group. DIAdem automatically adjusts the scaling of all axes that belong to the same synchronization group when you modify an axis scaling.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsynchronizationgroupint-id/">ID</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/synchronizationgroups/">SynchronizationGroups</a>.<a href="../../methods/irepsynchronizationgroupsint-add/">Add</a> | <a href="../../collections/synchronizationgroups/">SynchronizationGroups</a>.<a href="../../methods/irepsynchronizationgroupsint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSynchronizationGroupInt.htm`*
