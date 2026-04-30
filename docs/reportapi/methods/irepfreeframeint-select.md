---
title: "IRepFreeFrameInt.Select"
description: "Selects a rectangle in DIAdem REPORT."
---

# IRepFreeFrameInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for Frame

Selects a rectangle in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyFrame.Select()
dd.MsgBoxDisp(oMyFrame.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepFreeFrameInt.htm`*
