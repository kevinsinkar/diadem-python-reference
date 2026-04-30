---
title: "IRepTextSimpleInt.Font"
description: "Specifies the font attributes of a text in DIAdem REPORT."
---

# IRepTextSimpleInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for Text

Specifies the font attributes of a text in DIAdem REPORT.

## Signature

```python
return_value = obj.Font
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
oMyText.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepTextSimpleInt.htm`*
