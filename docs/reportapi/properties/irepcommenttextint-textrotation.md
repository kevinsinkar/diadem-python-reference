---
title: "IRepCommentTextInt.TextRotation"
description: "Specifies the angle of a comment in the comment frame in DIAdem REPORT."
---

# IRepCommentTextInt.TextRotation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TextRotation for CommentElement

Specifies the angle of a comment in the comment frame in DIAdem REPORT.

## Signature

```python
obj.TextRotation
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAngle0` | 0 |  |
| `eAngle090` | 1 | 90 |
| `eAngle180` | 2 | 180 |
| `eAngle270` | 3 | 270 |

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyComment.Comment.TextRotation = (dd.eAngle090)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TextRotation_IRepCommentTextInt.htm`*
