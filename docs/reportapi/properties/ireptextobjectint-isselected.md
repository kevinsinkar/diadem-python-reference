---
title: "IRepTextObjectInt.IsSelected"
description: "Specifies whether a Text object is selected in DIAdem REPORT."
---

# IRepTextObjectInt.IsSelected

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IsSelected for RTFText

Specifies whether a Text object is selected in DIAdem REPORT.

## Signature

```python
obj.IsSelected
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>With the object-oriented script interface in DIAdem REPORT, you can only create, position, and select text objects. You cannot create and change text in text objects.</td></tr></table>
</div>

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
sOutput = ""
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectRTFText :
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

*Source: `ReportApi/properties/Report_property_IsSelected_IRepTextObjectInt.htm`*
