---
title: "IRepSynchronizationGroupsInt.Item"
description: "Returns a synchronization group from the list of synchronization groups in DIAdem REPORT."
---

# IRepSynchronizationGroupsInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for SynchronizationGroups

Returns a synchronization group from the list of synchronization groups in DIAdem REPORT.

## Signature

```python
return_value = obj.Item(IDOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the Item method because it is the standard element of the collection.</td></tr></table>
</div>

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

*Source: `ReportApi/methods/Report_method_Item_IRepSynchronizationGroupsInt.htm`*
