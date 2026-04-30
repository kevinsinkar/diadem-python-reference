---
title: "IRepTextSimpleInt.Select"
description: "Selects a text in DIAdem REPORT."
---

# IRepTextSimpleInt.Select

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Select for Text

Selects a text in DIAdem REPORT.

## Signature

```python
obj.Select()
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "Test"
oMyText.Select()
dd.MsgBoxDisp(oMyText.IsSelected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Select_IRepTextSimpleInt.htm`*
