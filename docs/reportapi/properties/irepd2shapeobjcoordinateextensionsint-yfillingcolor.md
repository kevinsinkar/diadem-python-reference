---
title: "IRepD2ShapeObjCoordinateExtensionsInt.YFillingColor"
description: "Specifies the filling color between the vertical lines of the y-coordinate in a 2D axis system in the Coordinate display mode in DIAdem REPORT."
---

# IRepD2ShapeObjCoordinateExtensionsInt.YFillingColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YFillingColor for 2DCoordinateExtensions

Specifies the filling color between the vertical lines of the y-coordinate in a 2D axis system in the Coordinate display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.YFillingColor
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")

oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,"My2DCurveCoord")
oMyShape = oMyCurveCoord.Shape
oMyShape.X1Coordinate.Reference = 80
oMyShape.XCoordinate.Reference = 50
oMyShape.YCoordinate.Reference = 20
oMyShape.Y1Coordinate.Reference = 40
oMyShape.Settings.Type = dd.eMarkerCross
oMyShape.Settings.Size = 5

oMyExtensions = oMyShape.Extensions
oMyExtensions.XConstantLine.Color.ColorIndex = dd.eColorIndexBlack
oMyExtensions.YConstantLine.Color.ColorIndex = dd.eColorIndexBlack
oMyExtensions.XFillingColor.ColorIndex = dd.eColorIndexViolet
oMyExtensions.YFillingColor.ColorIndex = dd.eColorIndexGreen
oMyExtensions.XYFillingColor.ColorIndex = dd.eColorIndexGrey

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YFillingColor_IRepD2ShapeObjCoordinateExtensionsInt.htm`*
