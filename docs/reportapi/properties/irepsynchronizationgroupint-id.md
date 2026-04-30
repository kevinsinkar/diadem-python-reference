---
title: "IRepSynchronizationGroupInt.ID"
description: "Specifies the unique name of a synchronization group in DIAdem REPORT."
---

# IRepSynchronizationGroupInt.ID

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ID for SynchronizationGroup

Specifies the unique name of a synchronization group in DIAdem REPORT.

## Signature

```python
obj.ID
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

*Source: `ReportApi/properties/Report_property_ID_IRepSynchronizationGroupInt.htm`*
