---
title: "IRepBackgroundColorInt.RGBFilling"
description: "Specifies the RGB values of the second highlighting color of a color shading in DIAdem REPORT. First assign the value eColorIndexFillEffects to the property Col"
---

# IRepBackgroundColorInt.RGBFilling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RGBFilling for BackgroundColor

Specifies the RGB values of the second highlighting color of a color shading in DIAdem REPORT. First assign the value eColorIndexFillEffects to the property ColorIndex . The RGB property specifies the first color of a filling effect. You also can use the SetFillingColor method to specify filling effects. Not all REPORT objects support filling effects.

## Signature

```python
obj.RGBFilling
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
oMyText.Font.BackColor.ColorIndex = dd.eColorIndexFillEffects
oMyText.Font.BackColor.GradientDirection = dd.eColorGradientDiagonalLeft
oMyText.Font.BackColor.GradientMode = dd.eColorGradientModeFromBottom
oMyText.Font.BackColor.RGB = dd.RGB(255, 0, 0)
oMyText.Font.BackColor.RGBFilling = dd.RGB(0,255,0)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RGBFilling_IRepBackgroundColorInt.htm`*
