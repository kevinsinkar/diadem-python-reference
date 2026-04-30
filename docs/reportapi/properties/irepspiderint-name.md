---
title: "IRepSpiderInt.Name"
description: "Specifies the name of the selected object in a spider axis system in DIAdem REPORT."
---

# IRepSpiderInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for Spider

Specifies the name of the selected object in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectSpider :
        sOutput = sOutput + "Object " + oMyReportObj.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepSpiderInt.htm`*
