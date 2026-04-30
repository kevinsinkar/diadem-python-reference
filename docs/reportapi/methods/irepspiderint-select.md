---
title: "IRepSpiderInt.Select"
description: "Selects a spider axis system in DIAdem REPORT."
---

# IRepSpiderInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for Spider

Selects a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider,"MySpiderAxisSystem")
oMyAxisSystem.Select()
dd.MsgBoxDisp(oMyAxisSystem.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepSpiderInt.htm`*
