---
title: "IRepCommentInt.Arrow"
description: "Specifies the arrow that belongs to a comment in DIAdem REPORT."
---

# IRepCommentInt.Arrow

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Arrow for Comment

Specifies the arrow that belongs to a comment in DIAdem REPORT.

## Signature

```python
return_value = obj.Arrow
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
dd.MsgBoxDisp(oMyComment.Arrow.Line.Width)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Arrow_IRepCommentInt.htm`*
