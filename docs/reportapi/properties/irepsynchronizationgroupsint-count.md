---
title: "IRepSynchronizationGroupsInt.Count"
description: "Returns the number of synchronization groups in DIAdem REPORT."
---

# IRepSynchronizationGroupsInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for SynchronizationGroups

Returns the number of synchronization groups in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyXSync = dd.Report.Settings.Synchronization.AxisSystem2D.XAxis
for i in range( 1, oMyXSync.Count+1):
    sOutput = sOutput + oMyXSync.Item(i).ID + "\r\n"
print(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepSynchronizationGroupsInt.htm`*
