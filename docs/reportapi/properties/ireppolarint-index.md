---
title: "IRepPolarInt.Index"
description: "Returns the index of a polar axis system in DIAdem REPORT. If you change the ZOrder property of an object, you also change the indexes of all objects."
---

# IRepPolarInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for PolarSystem

Returns the index of a polar axis system in DIAdem REPORT. If you change the ZOrder property of an object, you also change the indexes of all objects.

## Signature

```python
obj.Index
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        sOutput = sOutput + "Object " + oMyReportObj.Name + ": Index: "+ oMyReportObj.Index + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepPolarInt.htm`*
