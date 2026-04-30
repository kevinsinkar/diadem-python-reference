---
title: "IRepD2ShapeObjConstantInt.Y1Constant"
description: "Specifies the y1-constant of a 2D axis system in the Constant display mode in DIAdem REPORT."
---

# IRepD2ShapeObjConstantInt.Y1Constant

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Y1Constant for 2DConstant

Specifies the y1-constant of a 2D axis system in the Constant display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Y1Constant
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80

oMyCurveConst = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeConstant, "MyConstant")
oMyCurveConst.Shape.XConstant.Reference = 10
oMyCurveConst.Shape.YConstant.Reference = 20
oMyCurveConst.Shape.X1Constant.Reference = 50
oMyCurveConst.Shape.Y1Constant.Reference = 80

oMySettings = oMyCurveConst.Shape.Settings
oMySettings.XFillingColor.ColorIndex = dd.eColorIndexViolet
oMySettings.YFillingColor.ColorIndex = dd.eColorIndexGreen
oMySettings.XYFillingColor.ColorIndex = dd.eColorIndexGrey

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Y1Constant_IRepD2ShapeObjConstantInt.htm`*
