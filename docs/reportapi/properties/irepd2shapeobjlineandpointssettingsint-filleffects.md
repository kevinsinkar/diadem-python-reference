---
title: "IRepD2ShapeObjLineAndPointsSettingsInt.FillEffects"
description: "Specifies the properties of the curve filling in the Line and points display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjLineAndPointsSettingsInt.FillEffects

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FillEffects for 2DLineAndPointsSettings

Specifies the properties of the curve filling in the Line and points display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.FillEffects
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyLabel = oMyShape.Extensions.Label
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.Position.Type = dd.e2DLabelPositionAtPoint
oMyLabel.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
oMySettings = oMyShape.Settings
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

*Source: `ReportApi/properties/Report_property_FillEffects_IRepD2ShapeObjLineAndPointsSettingsInt.htm`*
