---
title: "IRepD2ConstX1ObjectInt"
description: "The 2DConstantX1Object object provides the second x-constant of a curve in the display mode Constant in a 2D axis system in DIAdem REPORT."
---

# IRepD2ConstX1ObjectInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DConstantX1Object

The 2DConstantX1Object object provides the second x-constant of a curve in the display mode Constant in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")

oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeConstant, "MyNew2DCurve")
oMy2DCurve.Shape.XConstant.Reference = 10
oMy2DCurve.Shape.X1Constant.Reference = 80
oMy2DCurve.Shape.YConstant.Reference = 30
oMy2DCurve.Shape.Y1Constant.Reference = 70

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2constx1objectint-reference/">Reference</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjconstantint/">2DConstant</a>.<a href="../../properties/irepd2shapeobjconstantint-x1constant/">X1Constant</a> | <a href="../irepd2shapeobjcoordinateint/">2DCoordinate</a>.<a href="../../properties/irepd2shapeobjcoordinateint-x1coordinate/">X1Coordinate</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ConstX1ObjectInt.htm`*
