---
title: "IRepCommentTextInt.TextMargin"
description: "Specifies the distance between the comment and the comment frame as a percentage of the worksheet in cm or inch, in DIAdem REPORT."
---

# IRepCommentTextInt.TextMargin

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TextMargin for CommentElement

Specifies the distance between the comment and the comment frame as a percentage of the worksheet in cm or inch, in DIAdem REPORT.

## Signature

```python
obj.TextMargin
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyComment.Comment.TextMargin = 7
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TextMargin_IRepCommentTextInt.htm`*
