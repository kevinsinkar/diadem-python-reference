---
title: "IRepImageInt.Select"
description: "Selects a graphic in DIAdem REPORT."
---

# IRepImageInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for Image

Selects a graphic in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectImage,"MyImage")
oMyImage.Select()
dd.MsgBoxDisp(oMyImage.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepImageInt.htm`*
