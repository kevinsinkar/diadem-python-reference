---
title: "IRepD2ShapeObjConstantInt.Settings"
description: "Specifies the curve properties in the Constant display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjConstantInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 2DConstant

Specifies the curve properties in the Constant display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
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
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyLineShape = oMyCurveLine.Shape
oMyLineShape.XChannel.Reference = "[1]/[1]"
oMyLineShape.YChannel.Reference = "[1]/[2]"
oMyCurveConst = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeConstant, "MyConstant")
oMyConstShape = oMyCurveConst.Shape
oMyConstShape.XConstant.Reference = 10
oMyConstShape.YConstant.Reference = 20
oMySettings = oMyCurveConst.Shape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepD2ShapeObjConstantInt.htm`*
