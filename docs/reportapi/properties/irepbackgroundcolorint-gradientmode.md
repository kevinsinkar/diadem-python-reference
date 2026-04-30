---
title: "IRepBackgroundColorInt.GradientMode"
description: "Specifies the color shading variant of the highlighting color of an object in DIAdem REPORT. You also can use the SetFillingColor method to specify filling effe"
---

# IRepBackgroundColorInt.GradientMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: GradientMode for BackgroundColor

Specifies the color shading variant of the highlighting color of an object in DIAdem REPORT. You also can use the SetFillingColor method to specify filling effects. Not all REPORT objects display filling effects.

## Signature

```python
obj.GradientMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorGradientModeFromBottom` | 0 | From bottom |
| `eColorGradientModeFromTop` | 1 | From top |
| `eColorGradientModeFromInside` | 2 | From inside |
| `eColorGradientModeFromOutside` | 3 | From outside |
| `eColorGradientModeSectors` | 5 | Section wise |

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

*Source: `ReportApi/properties/Report_property_GradientMode_IRepBackgroundColorInt.htm`*
