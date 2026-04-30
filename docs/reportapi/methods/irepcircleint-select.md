---
title: "IRepCircleInt.Select"
description: "Selects a circle in DIAdem REPORT."
---

# IRepCircleInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for Circle

Selects a circle in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
oMyCircle.Select()
dd.MsgBoxDisp(oMyCircle.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepCircleInt.htm`*
