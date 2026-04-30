---
title: "IRepCommentInt.Name"
description: "Specifies the name of a comment in DIAdem REPORT."
---

# IRepCommentInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for Comment

Specifies the name of a comment in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
soutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectComment :
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

*Source: `ReportApi/properties/Report_property_Name_IRepCommentInt.htm`*
