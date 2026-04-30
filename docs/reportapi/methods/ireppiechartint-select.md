---
title: "IRepPieChartInt.Select"
description: "Selects a pie chart in DIAdem REPORT."
---

# IRepPieChartInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for PieChart

Selects a pie chart in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPieChart, "MyPieChart")
oMyAxisSystem.Select()
dd.MsgBoxDisp(oMyAxisSystem.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepPieChartInt.htm`*
