---
title: "IRepTextObjectInt.Index"
description: "Returns the index of a text object in DIAdem REPORT. If you change the ZOrder property of an object, you also change the indexes of all objects."
---

# IRepTextObjectInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for RTFText

Returns the index of a text object in DIAdem REPORT. If you change the ZOrder property of an object, you also change the indexes of all objects.

## Signature

```python
obj.Index
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>With the object-oriented script interface in DIAdem REPORT, you can only create, position, and select text objects. You cannot create and change text.</td></tr></table>
</div>

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectRTFText :
        sOutput = sOutput + "Object " + oMyReportObj.Name + ": Index: "+ oMyReportObj.Index + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepTextObjectInt.htm`*
