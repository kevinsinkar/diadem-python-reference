---
title: "IRepColorInt.Transparency"
description: "Specifies the percentaged transparency of a color in DIAdem REPORT. The value 100 specifies a completely transparent display and the value 0 specifies a complet"
---

# IRepColorInt.Transparency

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Transparency for Color

Specifies the percentaged transparency of a color in DIAdem REPORT. The value 100 specifies a completely transparent display and the value 0 specifies a completely opaque display. Not all DIAdem objects display transparency.

## Signature

```python
obj.Transparency
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
oMyColor.Transparency = 70
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Transparency_IRepColorInt.htm`*
