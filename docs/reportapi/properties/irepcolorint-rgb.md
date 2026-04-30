---
title: "IRepColorInt.RGB"
description: "Specifies the RGB values of a color in DIAdem REPORT. First assign the value eColorIndexOtherColors to the property ColorIndex . If you assign the value eColorI"
---

# IRepColorInt.RGB

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RGB for Color

Specifies the RGB values of a color in DIAdem REPORT. First assign the value eColorIndexOtherColors to the property ColorIndex . If you assign the value eColorIndexFillEffects to the property ColorIndex , the RGB property specifies the first color of a filling effect. You also can use the SetRGBColor method to specify individual colors. Use the SetFillingColor method to specify filling effects. Not all REPORT objects support filling effects.

## Signature

```python
obj.RGB
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMyXLine = oMy2DAxisSystem.XAxis.Line
oMyXLine.Color.ColorIndex = dd.eColorIndexOtherColors
oMyXLine.Color.RGB = dd.RGB(255, 0, 0)
oMyXLine.UseCurveColor = False
oMyYLine = oMy2DAxisSystem.YAxis.Line
oMyYLine.Color.SetRGBColor(dd.RGB(0, 0, 255))
oMyYLine.UseCurveColor = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RGB_IRepColorInt.htm`*
