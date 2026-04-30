---
title: "IRepCommentTextInt.Font"
description: "Specifies the font properties of a comment in DIAdem REPORT."
---

# IRepCommentTextInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for CommentElement

Specifies the font properties of a comment in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "My Comment"
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

*Source: `ReportApi/properties/Report_property_Font_IRepCommentTextInt.htm`*
