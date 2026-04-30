---
title: "IRepPolarCurveListInt.Exists"
description: "Checks whether a polar curve with a specific name already exists in a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveListInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for PolarCurves

Checks whether a polar curve with a specific name already exists in a polar axis system in DIAdem REPORT.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.Report.ActiveSheet.Objects(1).Curves.Exists("2DPolar1_Curve1"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Exists_IRepPolarCurveListInt.htm`*
