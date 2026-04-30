---
title: "IRepPolarCurveInt.Index"
description: "Returns the index of a curve in a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for PolarCurve

Returns the index of a curve in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.Index
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        oMySubObjects = oMyReportObj.CurvesPolar
        for i in range( 1, oMySubObjects.Count+1):
            sOutput = sOutput + "Curve Index: " + oMySubObjects.Item(i).Index + "\t" + "Curve name: " + oMySubObjects.Item(i).Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepPolarCurveInt.htm`*
