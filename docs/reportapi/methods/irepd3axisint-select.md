---
title: "IRepD3AxisInt.Select"
description: "Selects a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for 3DAxisSystem

Selects a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DAxisSystem.Select()
dd.MsgBoxDisp(oMy3DAxisSystem.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepD3AxisInt.htm`*
