---
title: "IRepCommentTextInt.BorderLine"
description: "Specifies the line of a comment frame in DIAdem REPORT."
---

# IRepCommentTextInt.BorderLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BorderLine for CommentElement

Specifies the line of a comment frame in DIAdem REPORT.

## Signature

```python
return_value = obj.BorderLine
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "MyComment"
oMyComment.Comment.BorderLine.Width = dd.eLineWidth0200
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BorderLine_IRepCommentTextInt.htm`*
