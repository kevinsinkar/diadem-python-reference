---
title: "IRepReportInt.Comment"
description: "Specifies a comment in DIAdem REPORT."
---

# IRepReportInt.Comment

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Comment for Report

Specifies a comment in DIAdem REPORT.

## Signature

```python
obj.Comment
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyFont = oMyComment.Comment.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 7
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Comment_IRepReportInt.htm`*
