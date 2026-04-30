---
title: "IRepD2ShapeObjConstantInt.Extensions"
description: "Specifies the extended properties of a curve in the Constant display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjConstantInt.Extensions

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Extensions for 2DConstant

Specifies the extended properties of a curve in the Constant display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Extensions
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
oMyConstantLabel = oMyConstShape.Extensions.ConstantLabel
oMyConstantLabel.Type = dd.e2DLabelCustomText
oMyConstantLabel.Text = "Point"
oMyConstantLabel.RelativePosition = dd.eRelativePositionLeftBottom
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

*Source: `ReportApi/properties/Report_property_Extensions_IRepD2ShapeObjConstantInt.htm`*
