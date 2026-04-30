---
title: "IRepFormulaDisplayInt.Select"
description: "Selects a formula graphic in DIAdem REPORT."
---

# IRepFormulaDisplayInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for FormulaDisplay

Selects a formula graphic in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyFormulaDisplay = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFormulaDisplay,"MyFormulaDisplay")
oMyFormulaDisplay.Select()
dd.MsgBoxDisp(oMyFormulaDisplay.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepFormulaDisplayInt.htm`*
