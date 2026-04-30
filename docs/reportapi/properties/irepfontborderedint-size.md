---
title: "IRepFontBorderedInt.Size"
description: "Specifies the font size of a text with a frame as a percentage of the page height in DIAdem REPORT."
---

# IRepFontBorderedInt.Size

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Size for FontWithBorder

Specifies the font size of a text with a frame as a percentage of the page height in DIAdem REPORT.

## Signature

```python
obj.Size
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Size_IRepFontBorderedInt.htm`*
