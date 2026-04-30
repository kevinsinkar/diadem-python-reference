---
title: "IRepD2AxisXInt.Name"
description: "Specifies the name of an x-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for 2DAxisX

Specifies the name of an x-axis in a 2D axis system in DIAdem REPORT.

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
        sOutput = sOutput + "Object " + oMyReportObj.XAxis.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepD2AxisXInt.htm`*
