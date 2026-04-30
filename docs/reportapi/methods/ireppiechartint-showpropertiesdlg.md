---
title: "IRepPieChartInt.ShowPropertiesDlg"
description: "Opens the dialog box where you specify the properties of a pie chart in DIAdem REPORT."
---

# IRepPieChartInt.ShowPropertiesDlg

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ShowPropertiesDlg for PieChart

Opens the dialog box where you specify the properties of a pie chart in DIAdem REPORT.

## Signature

```python
obj.ShowPropertiesDlg()
```

## Python example

```python
dd.Report.NewLayout()
oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPieChart, "MyPieChart")
oMyAxisSystem.ShowPropertiesDlg()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ShowPropertiesDlg_IRepPieChartInt.htm`*
