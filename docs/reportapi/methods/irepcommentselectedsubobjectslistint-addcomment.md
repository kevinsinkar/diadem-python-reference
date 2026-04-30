---
title: "IRepCommentSelectedSubObjectsListInt.AddComment"
description: "Selects the subobject of a comment in DIAdem REPORT associated with a specific index. In order to select an individual frame line, enable the property UseIndivi"
---

# IRepCommentSelectedSubObjectsListInt.AddComment

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: AddComment for CommentSelectedElements

Selects the subobject of a comment in DIAdem REPORT associated with a specific index. In order to select an individual frame line, enable the property UseIndividualLineStyle .

## Signature

```python
return_value = obj.AddComment(ElementType, Index)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCommentElementArrow` | 0 | Arrow |
| `eCommentFrameTop` | 1 | Upper frame |
| `eCommentFrameBottom` | 2 | Lower frame |
| `eCommentFrameLeft` | 3 | Left frame |
| `eCommentFrameRight` | 4 | Right frame |

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyFrameLine = oMyComment.Comment.BorderLine
oMyLineIndividual = oMyFrameLine.LineBottom
oMyFrameLine.UseIndividualLineStyle  = True

oMyComment.SelectedElements.AddComment(dd.eCommentFrameTop , 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_AddComment_IRepCommentSelectedSubObjectsListInt.htm`*
