---
title: "IRepFontInt.Name"
description: "Specifies the name of a font in DIAdem REPORT."
---

# IRepFontInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for Font

Specifies the name of a font in DIAdem REPORT.

## Signature

```python
obj.Name
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
sOutput = "Used fonts in comment objects" + "\r\n"
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectComment :
        sOutput = sOutput + oMyReportObj.Comment.Font.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepFontInt.htm`*
