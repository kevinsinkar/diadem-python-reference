---
title: "IRepD2ConstX1ObjectInt.Reference"
description: "Specifies the reference to the second x-constant of a curve in the Constant display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ConstX1ObjectInt.Reference

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Reference for 2DConstantX1Object

Specifies the reference to the second x-constant of a curve in the Constant display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Reference
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

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeConstant, "MyNew2DCurve")
oMy2DCurve.Shape.XConstant.Reference = 10
oMy2DCurve.Shape.X1Constant.Reference = 80
oMy2DCurve.Shape.YConstant.Reference = 30
oMy2DCurve.Shape.Y1Constant.Reference = 70

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Reference_IRepD2ConstX1ObjectInt.htm`*
