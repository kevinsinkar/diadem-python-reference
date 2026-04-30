---
title: "IRepBackgroundColorInt.Transparency"
description: "Specifies the transparency of a highlighting color as a percentage in DIAdem REPORT. The value 100 specifies a completely transparent display and the value 0 sp"
---

# IRepBackgroundColorInt.Transparency

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Transparency for BackgroundColor

Specifies the transparency of a highlighting color as a percentage in DIAdem REPORT. The value 100 specifies a completely transparent display and the value 0 specifies a completely opaque display. Not all DIAdem objects display transparency.

## Signature

```python
obj.Transparency
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
oMyText.Font.BackColor.SetPredefinedColor(dd.ePredefinedColorDarkRed)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Transparency_IRepBackgroundColorInt.htm`*
