---
title: "IRepArrowInt.Select"
description: "Selects an arrow in DIAdem REPORT."
---

# IRepArrowInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for Arrow

Selects an arrow in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyArrow = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectArrow,"MyArrow")
oMyArrow.Select()
dd.MsgBoxDisp(oMyArrow.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepArrowInt.htm`*
