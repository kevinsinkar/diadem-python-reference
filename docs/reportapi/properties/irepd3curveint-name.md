---
title: "IRepD3CurveInt.Name"
description: "Specifies the name of a curve in a 3D axis system in DIAdem REPORT."
---

# IRepD3CurveInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for 3DCurve

Specifies the name of a curve in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        for oMyCurve in oMyReportObj.Curves3D:
            sOutput = sOutput + "Object " + oMyCurve.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepD3CurveInt.htm`*
