---
title: "IRepD2ShapeObjCoordinateExtensionsInt.CoordinateLabel"
description: "Specifies the properties of the coordinate label in 2D axis systems with the Coordinate display mode in DIAdem REPORT."
---

# IRepD2ShapeObjCoordinateExtensionsInt.CoordinateLabel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CoordinateLabel for 2DCoordinateExtensions

Specifies the properties of the coordinate label in 2D axis systems with the Coordinate display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.CoordinateLabel
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
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurveLine")
oMyCurveLine.Shape.XChannel.Reference = "[1]/[1]"
oMyCurveLine.Shape.YChannel.Reference = "[1]/[2]"

oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,"My2DCurveCoord")
MaxValY = dd.Data.GetChannel("[1]/[2]").Properties("maximum").Value
MaxValX = dd.Data.GetChannel("[1]/[1]").Values(dd.PNo("[1]/[2]", MaxValY))
oMyShape = oMyCurveCoord.Shape
oMyShape.BoundingType = dd.eCoordinateChannelBounded
oMyShape.BoundingPosition = dd.e2DCoordinateBoundingAbsoluteMax
oMyShape.BoundingXChannel.Reference = "[1]/[1]"
oMyShape.BoundingyChannel.Reference = "[1]/[2]"
oMyShape.Settings.Type = dd.eMarkerCircle

oMyShape.XCoordinate.Reference = MaxValX
oMyShape.YCoordinate.Reference = MaxValY

oMyCoordLabel = oMyShape.Extensions.CoordinateLabel
oMyCoordLabel.Type = dd.e2DLabelValue
oMyCoordLabel.UseXPositionOffset = True
oMyCoordLabel.UseYPositionOffset = True
oMyCoordLabel.XPositionOffset = 5
oMyCoordLabel.YPositionOffset = 5
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CoordinateLabel_IRepD2ShapeObjCoordinateExtensionsInt.htm`*
