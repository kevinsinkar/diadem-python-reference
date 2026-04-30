---
title: "IRepColorInt.GradientMode"
description: "Specifies the color shading direction in DIAdem REPORT. You also can use the SetFillingColor method to specify filling effects. Not all REPORT objects display f"
---

# IRepColorInt.GradientMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: GradientMode for Color

Specifies the color shading direction in DIAdem REPORT. You also can use the SetFillingColor method to specify filling effects. Not all REPORT objects display filling effects.

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

*Source: `ReportApi/properties/Report_property_GradientMode_IRepColorInt.htm`*
