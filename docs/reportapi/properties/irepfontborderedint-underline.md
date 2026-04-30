---
title: "IRepFontBorderedInt.Underline"
description: "Specifies whether DIAdem REPORT uses underline font to display text."
---

# IRepFontBorderedInt.Underline

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Underline for FontWithBorder

Specifies whether DIAdem REPORT uses underline font to display text.

## Signature

```python
obj.Underline
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "This is a Text"
oMyFont = oMyText.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 10
oMyFont.Border = True
oMyFont.Underline = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Underline_IRepFontBorderedInt.htm`*
