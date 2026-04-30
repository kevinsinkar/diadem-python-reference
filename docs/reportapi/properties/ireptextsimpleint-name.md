---
title: "IRepTextSimpleInt.Name"
description: "Specifies the name of a text in DIAdem REPORT."
---

# IRepTextSimpleInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for Text

Specifies the name of a text in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectText :
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

*Source: `ReportApi/properties/Report_property_Name_IRepTextSimpleInt.htm`*
