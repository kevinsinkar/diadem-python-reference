---
title: "IRepCommentInt.Select"
description: "Selects a comment in DIAdem REPORT."
---

# IRepCommentInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for Comment

Selects a comment in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Select()
dd.MsgBoxDisp(oMyComment.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepCommentInt.htm`*
