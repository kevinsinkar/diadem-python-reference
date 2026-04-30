---
title: "IRepFillEffectsInt.PatternType"
description: "Specifies the pattern type for the filled area of a 2D axis system in DIAdem REPORT."
---

# IRepFillEffectsInt.PatternType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PatternType for FillEffects

Specifies the pattern type for the filled area of a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.PatternType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eFillPatternTypeThin` | 0 | Thin |
| `eFillPatternTypeThick` | 1 | Thick |
| `eFillPatternTypeWide` | 2 | Wide |

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
oMyFillEffect.PatternType = dd.eFillPatternTypeThick
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PatternType_IRepFillEffectsInt.htm`*
