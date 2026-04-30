---
title: "IRepSettingsInt.Synchronization"
description: "Specifies the properties for synchronizing axes in DIAdem REPORT."
---

# IRepSettingsInt.Synchronization

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Synchronization for Settings

Specifies the properties for synchronizing axes in DIAdem REPORT.

## Signature

```python
return_value = obj.Synchronization
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

*Source: `ReportApi/properties/Report_property_Synchronization_IRepSettingsInt.htm`*
