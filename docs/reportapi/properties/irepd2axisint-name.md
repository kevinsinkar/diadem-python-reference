---
title: "IRepD2AxisInt.Name"
description: "Specifies the name of a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for 2DAxisSystem

Specifies the name of a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        sOutput = sOutput + "Object " + oMyReportObj.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepD2AxisInt.htm`*
