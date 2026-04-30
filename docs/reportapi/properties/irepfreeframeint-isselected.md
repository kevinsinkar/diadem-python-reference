---
title: "IRepFreeFrameInt.IsSelected"
description: "Specifies whether a rectangle is selected in DIAdem REPORT."
---

# IRepFreeFrameInt.IsSelected

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IsSelected for Frame

Specifies whether a rectangle is selected in DIAdem REPORT.

## Signature

```python
obj.IsSelected
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
sOutput = ""
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectFrame :
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

*Source: `ReportApi/properties/Report_property_IsSelected_IRepFreeFrameInt.htm`*
