---
title: "IRepD2ShapeObjLineSettingsInt.FillEffects"
description: "Specifies the filling properties of a curve in the Lines display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjLineSettingsInt.FillEffects

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FillEffects for 2DLineSettings

Specifies the filling properties of a curve in the Lines display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.FillEffects
```

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
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

*Source: `ReportApi/properties/Report_property_FillEffects_IRepD2ShapeObjLineSettingsInt.htm`*
