---
title: "IRepD3CurveInt.Index"
description: "Returns the index of a curve in a 3D axis system in DIAdem REPORT."
---

# IRepD3CurveInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for 3DCurve

Returns the index of a curve in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Index
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        oMySubObjects = oMyReportObj.Curves3D
        for i in range( 1, oMySubObjects.Count+1):
            sOutput = sOutput + "Curve shape: " + oMySubObjects.Item(i).ShapeType + "\t" + "Curve name: " + oMySubObjects.Item(i).Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepD3CurveInt.htm`*
