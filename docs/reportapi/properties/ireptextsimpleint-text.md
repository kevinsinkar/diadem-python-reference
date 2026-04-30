---
title: "IRepTextSimpleInt.Text"
description: "Specifies a text in DIAdem REPORT."
---

# IRepTextSimpleInt.Text

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Text for Text

Specifies a text in DIAdem REPORT.

## Signature

```python
obj.Text
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Text_IRepTextSimpleInt.htm`*
