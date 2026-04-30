---
title: "IRepCommentSelectedSubObjInt"
description: "The CommentSelectedElement object provides a selected element from a comment in DIAdem REPORT."
---

# IRepCommentSelectedSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CommentSelectedElement

The CommentSelectedElement object provides a selected element from a comment in DIAdem REPORT.

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectComment :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of selected elements: " + oMyReportObj.SelectedElements.Count)
        for oMySelection in oMyReportObj.SelectedElements:
            sOutput = sOutput + "Element type: " + oMySelection.Type + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcommentselectedsubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/commentselectedelements/">CommentSelectedElements</a>.<a href="../../methods/irepcommentselectedsubobjectslistint-addcomment/">AddComment</a> | <a href="../../collections/commentselectedelements/">CommentSelectedElements</a>.<a href="../../methods/irepcommentselectedsubobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCommentSelectedSubObjInt.htm`*
