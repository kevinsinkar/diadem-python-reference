---
title: "IRepFillEffectsInt.GradientMode"
description: "Specifies whether filling effects in DIAdem REPORT relate to the curve or to the axis. If the filling effect relates to the axis, DIAdem REPORT does not use the"
---

# IRepFillEffectsInt.GradientMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: GradientMode for FillEffects

Specifies whether filling effects in DIAdem REPORT relate to the curve or to the axis. If the filling effect relates to the axis, DIAdem REPORT does not use the entire color spectrum of a color shading for shorter curves. In this case, however, it is easier to compare different curves.

## Signature

```python
obj.GradientMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eFillGradientAxisRelated` | 0 | Axis related |
| `eFillGradientCurveRelated` | 1 | Curve related |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyScaling = oMy2DAxisSystem.XAxis.Scaling
oMyScaling.AutoScalingType = dd.eAxisAutoScalingBeginEndManual
oMyScaling.End = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySettings = oMyShape.Settings
oMyFillEffect = oMySettings.FillEffects
oMyFillEffect.Color.SetFillingColor(255, 0, dd.eColorGradientHorizontal, dd.eColorGradientModeFromInside)
oMyFillEffect.Pattern = dd.eFillPatternFilled
oMyFillEffect.GradientMode = dd.eFillGradientAxisRelated
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_GradientMode_IRepFillEffectsInt.htm`*
