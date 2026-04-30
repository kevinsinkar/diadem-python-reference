---
title: "CommentSelectedElements"
description: "Collection of all CommentSelectedElement objects in DIAdem REPORT. Use the CommentSelectedElements collection to access a selected element of the comment."
---

# CommentSelectedElements

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: CommentSelectedElements

Collection of all CommentSelectedElement objects in DIAdem REPORT. Use the CommentSelectedElements collection to access a selected element of the comment.

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
<p><a href="../../properties/irepcommentselectedsubobjectslistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepcommentselectedsubobjectslistint-addcomment/">AddComment</a> | <a href="../../methods/irepcommentselectedsubobjectslistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepcommentint/">Comment</a>.<a href="../../properties/irepcommentint-selectedelements/">SelectedElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCommentSelectedSubObjectsListInt.htm`*
