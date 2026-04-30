---
title: "IRepFontBorderedInt.BackColor"
description: "Specifies the background color of a text in DIAdem REPORT. The text might be, for example, the label of an axis or of a text object."
---

# IRepFontBorderedInt.BackColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackColor for FontWithBorder

Specifies the background color of a text in DIAdem REPORT. The text might be, for example, the label of an axis or of a text object.

## Signature

```python
return_value = obj.BackColor
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
oMyFont.BackColor.ColorIndex = dd.eColorIndexYellow
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackColor_IRepFontBorderedInt.htm`*
