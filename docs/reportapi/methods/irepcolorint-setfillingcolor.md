---
title: "IRepColorInt.SetFillingColor"
description: "Specifies the filling effects of an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display the filling ef"
---

# IRepColorInt.SetFillingColor

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetFillingColor for Color

Specifies the filling effects of an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display the filling effects. Not all REPORT objects display filling effects.

## Signature

```python
obj.SetFillingColor(RGB1, RGB2, GradientDirection, GradientMode)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorGradientHorizontal` | 0 | Horizontal |
| `eColorGradientVertical` | 1 | Vertical |
| `eColorGradientDiagonalLeft` | 2 | Diagonal left |
| `eColorGradientDiagonalRight` | 3 | Diagonal right |
| `eColorGradientModeFromBottom` | 0 | From bottom |
| `eColorGradientModeFromTop` | 1 | From top |
| `eColorGradientModeFromInside` | 2 | From inside |
| `eColorGradientModeFromOutside` | 3 | From outside |
| `eColorGradientModeSectors` | 5 | Section wise |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeFilledArea, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
oMyFillEffect = oMySettings.FillEffects
oMyFillEffect.Color.SetFillingColor(255,0,dd.eColorGradientDiagonalRight,dd.eColorGradientModeFromInside)
oMyFillEffect.Pattern = dd.eFillPatternLeftDiagonal
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetFillingColor_IRepColorInt.htm`*
