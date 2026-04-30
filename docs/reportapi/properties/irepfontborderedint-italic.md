---
title: "IRepFontBorderedInt.Italic"
description: "Specifies whether DIAdem REPORT displays text in italics."
---

# IRepFontBorderedInt.Italic

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Italic for FontWithBorder

Specifies whether DIAdem REPORT displays text in italics.

## Signature

```python
obj.Italic
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "This is a text"
oMyFont = oMyText.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 10
oMyFont.Border = True
oMyFont.Italic = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Italic_IRepFontBorderedInt.htm`*
