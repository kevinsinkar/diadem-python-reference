---
title: "IRepD2ShapeObjConstantInt"
description: "The 2DConstant object provides the curve properties of a 2D axis system in the Constant display mode in DIAdem REPORT."
---

# IRepD2ShapeObjConstantInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DConstant

The 2DConstant object provides the curve properties of a 2D axis system in the Constant display mode in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjconstantint-extensions/">Extensions</a> | <a href="../../properties/irepd2shapeobjconstantint-settings/">Settings</a> | <a href="../../properties/irepd2shapeobjconstantint-x1constant/">X1Constant</a> | <a href="../../properties/irepd2shapeobjconstantint-xconstant/">XConstant</a> | <a href="../../properties/irepd2shapeobjconstantint-y1constant/">Y1Constant</a> | <a href="../../properties/irepd2shapeobjconstantint-yconstant/">YConstant</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2curveint/">2DCurve</a>.<a href="../../properties/irepd2curveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjConstantInt.htm`*
