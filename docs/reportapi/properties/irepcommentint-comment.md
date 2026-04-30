---
title: "IRepCommentInt.Comment"
description: "Specifies the properties of a comment in DIAdem REPORT."
---

# IRepCommentInt.Comment

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Comment for Comment

Specifies the properties of a comment in DIAdem REPORT.

## Signature

```python
return_value = obj.Comment
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "MyComment"
oMyComment.Comment.Font.Bold = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Comment_IRepCommentInt.htm`*
