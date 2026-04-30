---
title: "IRepCommentSelectedSubObjectsListInt.Count"
description: "Returns the number of selected elements of a comment in DIAdem REPORT."
---

# IRepCommentSelectedSubObjectsListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for CommentSelectedElements

Returns the number of selected elements of a comment in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectComment :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of selected elements: " + oMyReportObj.SelectedElements.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepCommentSelectedSubObjectsListInt.htm`*
