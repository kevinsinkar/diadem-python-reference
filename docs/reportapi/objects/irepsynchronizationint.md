---
title: "IRepSynchronizationInt"
description: "The Synchronization object provides properties for synchronizing axes in DIAdem REPORT."
---

# IRepSynchronizationInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Synchronization

The Synchronization object provides properties for synchronizing axes in DIAdem REPORT.

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
<p><a href="../../properties/irepsynchronizationint-axissystem2d/">AxisSystem2D</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsint/">Settings</a>.<a href="../../properties/irepsettingsint-synchronization/">Synchronization</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSynchronizationInt.htm`*
