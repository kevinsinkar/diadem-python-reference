---
title: "IRepD2CurveListInt.Exists"
description: "Checks whether a 2D curve with a specific name already exists in a 2D axis system in DIAdem REPORT."
---

# IRepD2CurveListInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for 2DCurves

Checks whether a 2D curve with a specific name already exists in a 2D axis system in DIAdem REPORT.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.Report.ActiveSheet.Objects(1).Curves2D.Exists("2D_Curve1"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Exists_IRepD2CurveListInt.htm`*
