---
title: "IRepPolarInt.Select"
description: "Selects a polar axis system in DIAdem REPORT."
---

# IRepPolarInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for PolarSystem

Selects a polar axis system in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(eReportObjectPolarAxisSystem,"MyPolarAxisSystem")
oMyPolarAxisSystem.Select()
dd.MsgBoxDisp(oMyPolarAxisSystem.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepPolarInt.htm`*
