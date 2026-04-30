---
title: "IRepD3CurveListInt.Exists"
description: "Checks whether a 3D curve with a specific name already exists in a 3D axis system in DIAdem REPORT."
---

# IRepD3CurveListInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for 3DCurves

Checks whether a 3D curve with a specific name already exists in a 3D axis system in DIAdem REPORT.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.Report.ActiveSheet.Objects(1).Curves3D.Exists("3D_Curve1"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Exists_IRepD3CurveListInt.htm`*
