---
title: "IRepCommentTextInt.TextAlignmentHorizontal"
description: "Specifies the horizontal alignment of a comment in the comment frame in DIAdem REPORT."
---

# IRepCommentTextInt.TextAlignmentHorizontal

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TextAlignmentHorizontal for CommentElement

Specifies the horizontal alignment of a comment in the comment frame in DIAdem REPORT.

## Signature

```python
obj.TextAlignmentHorizontal
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCommentTextAlignmentHorizontalLeft` | 0 | Left |
| `eCommentTextAlignmentHorizontalCentric` | 1 | Center |
| `eCommentTextAlignmentHorizontalRight` | 2 | Right |

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyComment.Comment.TextAlignmentHorizontal = dd.eCommentTextAlignmentHorizontalRight
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TextAlignmentHorizontal_IRepCommentTextInt.htm`*
