---
title: "IRepCommentTextInt.TextAlignmentVertical"
description: "Specifies the vertical alignment of a comment in the comment frame in DIAdem REPORT."
---

# IRepCommentTextInt.TextAlignmentVertical

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TextAlignmentVertical for CommentElement

Specifies the vertical alignment of a comment in the comment frame in DIAdem REPORT.

## Signature

```python
obj.TextAlignmentVertical
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCommentTextAlignmentVerticalTop` | 0 | Top |
| `eCommentTextAlignmentVerticalCentric` | 1 | Center |
| `eCommentTextAlignmentVerticalBottom` | 2 | Bottom |

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyComment.Comment.TextAlignmentVertical = dd.eCommentTextAlignmentVerticalBottom
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TextAlignmentVertical_IRepCommentTextInt.htm`*
