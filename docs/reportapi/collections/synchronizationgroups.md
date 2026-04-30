---
title: "SynchronizationGroups"
description: "Collection of SynchronizationGroup objects in DIAdem REPORT. DIAdem automatically adjusts the scaling of all axes that belong to the same synchronization group "
---

# SynchronizationGroups

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: SynchronizationGroups

Collection of SynchronizationGroup objects in DIAdem REPORT. DIAdem automatically adjusts the scaling of all axes that belong to the same synchronization group when you modify an axis scaling.

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
<p><a href="../../properties/irepsynchronizationgroupsint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepsynchronizationgroupsint-add/">Add</a> | <a href="../../methods/irepsynchronizationgroupsint-exists/">Exists</a> | <a href="../../methods/irepsynchronizationgroupsint-item/">Item</a> | <a href="../../methods/irepsynchronizationgroupsint-remove/">Remove</a> | <a href="../../methods/irepsynchronizationgroupsint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepsynchronizationaxissystem2dint/">SynchronizationAxisSystem2D</a>.<a href="../../properties/irepsynchronizationaxissystem2dint-xaxis/">XAxis</a> | <a href="../../objects/irepsynchronizationaxissystem2dint/">SynchronizationAxisSystem2D</a>.<a href="../../properties/irepsynchronizationaxissystem2dint-yaxis/">YAxis</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSynchronizationGroupsInt.htm`*
