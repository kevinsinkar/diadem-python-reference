---
title: "IRepSpiderCurveListInt.Exists"
description: "Checks whether a curve with a specific name already exists in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveListInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for SpiderCurves

Checks whether a curve with a specific name already exists in a spider axis system in DIAdem REPORT.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.Report.ActiveSheet.Objects(1).CurvesSpider.Exists("Spider_Curve1"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Exists_IRepSpiderCurveListInt.htm`*
