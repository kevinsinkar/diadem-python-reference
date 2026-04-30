---
title: "IRepTable3DInt.Select"
description: "Selects a 3D table in DIAdem REPORT."
---

# IRepTable3DInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for 3DTable

Selects a 3D table in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMy3DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DTable,"My3DTable")
oMy3DTable.Select()
dd.MsgBoxDisp(oMy3DTable.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepTable3DInt.htm`*
