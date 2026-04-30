---
title: "IRepSynchronizationAxisSystem2DInt"
description: "The SynchronizationAxisSystem2D object provides properties for synchronizing axes of 2D axis systems in DIAdem REPORT."
---

# IRepSynchronizationAxisSystem2DInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SynchronizationAxisSystem2D

The SynchronizationAxisSystem2D object provides properties for synchronizing axes of 2D axis systems in DIAdem REPORT.

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
<p><a href="../../properties/irepsynchronizationaxissystem2dint-xaxis/">XAxis</a> | <a href="../../properties/irepsynchronizationaxissystem2dint-yaxis/">YAxis</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsynchronizationint/">Synchronization</a>.<a href="../../properties/irepsynchronizationint-axissystem2d/">AxisSystem2D</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSynchronizationAxisSystem2DInt.htm`*
