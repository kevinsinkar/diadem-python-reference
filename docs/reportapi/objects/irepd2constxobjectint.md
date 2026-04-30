---
title: "IRepD2ConstXObjectInt"
description: "The 2DConstantXObject object provides the value reference for the x-value of a constant or of a coordinate in 2D axis systems in DIAdem REPORT. You can specify "
---

# IRepD2ConstXObjectInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DConstantXObject

The 2DConstantXObject object provides the value reference for the x-value of a constant or of a coordinate in 2D axis systems in DIAdem REPORT. You can specify the value of the constant as a value or as a variable reference.

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
oMyCurveLine.Shape.XChannel.Reference = "[1]/[1]"
oMyCurveLine.Shape.YChannel.Reference = "[1]/[2]"
oMyCurveConst = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeConstant, "MyConstant")
oMyCurveConst.Shape.XConstant.Reference = 10
oMyCurveConst.Shape.YConstant.Reference = 20
oMySettings = oMyCurveConst.Shape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2constxobjectint-reference/">Reference</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjconstantint/">2DConstant</a>.<a href="../../properties/irepd2shapeobjconstantint-xconstant/">XConstant</a> | <a href="../irepd2shapeobjcoordinateint/">2DCoordinate</a>.<a href="../../properties/irepd2shapeobjcoordinateint-xcoordinate/">XCoordinate</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ConstXObjectInt.htm`*
