---
title: "IRepCommentSelectedSubObjInt.Type"
description: "Specifies the type of the selected element in a comment in DIAdem REPORT."
---

# IRepCommentSelectedSubObjInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for CommentSelectedElement

Specifies the type of the selected element in a comment in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCommentElementArrow` | 0 | Arrow |
| `eCommentElementTop` | 1 | Upper frame |
| `eCommentElementBottom` | 2 | Lower frame |
| `eCommentElementLeft` | 3 | Left frame |
| `eCommentElementRight` | 4 | Right frame |

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectComment :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of selected elements: " + oMyReportObj.SelectedElements.Count)
        for oMySelection in oMyReportObj.SelectedElements:
            sOutput = sOutput + "Element type: " + oMySelection.Type + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepCommentSelectedSubObjInt.htm`*
