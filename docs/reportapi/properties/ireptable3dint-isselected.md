---
title: "IRepTable3DInt.IsSelected"
description: "Specifies whether a 3D table is selected in DIAdem REPORT. The selected element can never be the main object and the Type can never have the value -1 ."
---

# IRepTable3DInt.IsSelected

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IsSelected for 3DTable

Specifies whether a 3D table is selected in DIAdem REPORT. The selected element can never be the main object and the Type can never have the value -1 .

## Signature

```python
obj.IsSelected
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
sOutput = ""
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DTable :
        sOutput = sOutput + "Object " + oMyReportObj.Name + " is selected: "+ oMyReportObj.IsSelected + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IsSelected_IRepTable3DInt.htm`*
