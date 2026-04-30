---
title: "IRepD2AxisInt.Select"
description: "Selects a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for 2DAxisSystem

Selects a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DAxisSystem.Select()
dd.MsgBoxDisp(oMy2DAxisSystem.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepD2AxisInt.htm`*
