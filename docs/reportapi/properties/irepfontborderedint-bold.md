---
title: "IRepFontBorderedInt.Bold"
description: "Specifies whether DIAdem REPORT displays text in bold type."
---

# IRepFontBorderedInt.Bold

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Bold for FontWithBorder

Specifies whether DIAdem REPORT displays text in bold type.

## Signature

```python
obj.Bold
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
oMyFont.Bold = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Bold_IRepFontBorderedInt.htm`*
