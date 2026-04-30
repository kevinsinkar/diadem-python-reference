---
title: "IRepTextObjectInt.Select"
description: "Selects a text object in DIAdem REPORT."
---

# IRepTextObjectInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for RTFText

Selects a text object in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyRtfText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectRtfText,"MyRtfText")
oMyRtfText.Select()
dd.MsgBoxDisp(oMyRtfText.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepTextObjectInt.htm`*
