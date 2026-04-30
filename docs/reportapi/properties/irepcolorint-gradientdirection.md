---
title: "IRepColorInt.GradientDirection"
description: "Specifies the color shading direction in DIAdem REPORT. You also can use the SetFillingColor method to specify filling effects. Not all REPORT objects display f"
---

# IRepColorInt.GradientDirection

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: GradientDirection for Color

Specifies the color shading direction in DIAdem REPORT. You also can use the SetFillingColor method to specify filling effects. Not all REPORT objects display filling effects.

## Signature

```python
obj.GradientDirection
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorGradientHorizontal` | 0 | Horizontal |
| `eColorGradientVertical` | 1 | Vertical |
| `eColorGradientDiagonalLeft` | 2 | Diagonal left |
| `eColorGradientDiagonalRight` | 3 | Diagonal right |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_GradientDirection_IRepColorInt.htm`*
