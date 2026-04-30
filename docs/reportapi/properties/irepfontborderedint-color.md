---
title: "IRepFontBorderedInt.Color"
description: "Specifies the font color in DIAdem REPORT. DIAdem only includes the Color property in the AxisLabel object if you assign the property FALSE to the UseCurveColor"
---

# IRepFontBorderedInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for FontWithBorder

Specifies the font color in DIAdem REPORT. DIAdem only includes the Color property in the AxisLabel object if you assign the property FALSE to the UseCurveColor property. DIAdem only includes the Color property in the AdditionalConstantLabel object if you assign the property FALSE to the UseLineColor property. DIAdem only includes the Color property in the AdditionalCoordinateLabel object if you assign the property FALSE to the UseMarkerColor property.

## Signature

```python
return_value = obj.Color
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

*Source: `ReportApi/properties/Report_property_Color_IRepFontBorderedInt.htm`*
