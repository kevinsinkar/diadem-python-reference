---
title: "IRepD2ShapeObjConstantSettingsInt.Palette"
description: "Specifies the palette properties of a curve in the Constant display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjConstantSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 2DConstantSettings

Specifies the palette properties of a curve in the Constant display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Palette
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurveLine.Shape.XChannel.Reference = "[1]/[1]"
oMyCurveLine.Shape.YChannel.Reference = "[1]/[2]"
oMyCurveConst = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeConstant, "MyConstant")
oMyCurveConst.Shape.XConstant.Reference = 10
oMyCurveConst.Shape.YConstant.Reference = 20
oMySettings = oMyCurveConst.Shape.Settings
oMySettings.Palette.ValueType = dd.e2DPaletteValueTypeDistanceOfAxisTicks
oMySettings.Line.Color.ColorIndex = dd.eColorIndexPalette
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepD2ShapeObjConstantSettingsInt.htm`*
