---
title: "IRepFontBorderedInt.Border"
description: "Specifies whether DIAdem REPORT frames a text."
---

# IRepFontBorderedInt.Border

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Border for FontWithBorder

Specifies whether DIAdem REPORT frames a text.

## Signature

```python
obj.Border
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Border_IRepFontBorderedInt.htm`*
