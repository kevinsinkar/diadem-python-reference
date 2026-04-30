---
title: "IRepTable2DInt.Select"
description: "Selects a 2D table in DIAdem REPORT."
---

# IRepTable2DInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for 2DTable

Selects a 2D table in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMy2DTable.Select()
dd.MsgBoxDisp(oMy2DTable.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepTable2DInt.htm`*
