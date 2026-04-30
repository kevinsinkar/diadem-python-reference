---
title: "IRepSynchronizationGroupsInt.Remove"
description: "Deletes a synchronization group from the list of synchronization groups in DIAdem REPORT."
---

# IRepSynchronizationGroupsInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for SynchronizationGroups

Deletes a synchronization group from the list of synchronization groups in DIAdem REPORT.

## Signature

```python
obj.Remove(IDOrIndex)
```

## Python example

```python
oMyXSync = dd.Report.Settings.Synchronization.AxisSystem2D.XAxis
if oMyXSync.Exists("XAxis Group1") :
    oMyXSync.Remove("XAxis Group1")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepSynchronizationGroupsInt.htm`*
