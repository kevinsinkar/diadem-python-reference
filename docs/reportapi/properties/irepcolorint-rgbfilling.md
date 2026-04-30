---
title: "IRepColorInt.RGBFilling"
description: "Specifies the RGB values of the second background color of a color shading in DIAdem REPORT. First assign the value eColorIndexFillEffects to the property Color"
---

# IRepColorInt.RGBFilling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RGBFilling for Color

Specifies the RGB values of the second background color of a color shading in DIAdem REPORT. First assign the value eColorIndexFillEffects to the property ColorIndex . The RGB property specifies the first color of a filling effect. You also can use the SetFillingColor method to specify filling effects. Not all REPORT objects support filling effects.

## Signature

```python
obj.RGBFilling
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyColor = oMy2DAxisSystem.Settings.BackgroundColor
oMyColor.ColorIndex = dd.eColorIndexFillEffects
oMyColor.RGBFilling = dd.RGB(147, 225, 225)
oMyColor.RGB = dd.RGB(255, 225, 0)
oMyColor.GradientDirection = dd.eColorGradientHorizontal
oMyColor.GradientMode = dd.eColorGradientModeFromInside
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RGBFilling_IRepColorInt.htm`*
