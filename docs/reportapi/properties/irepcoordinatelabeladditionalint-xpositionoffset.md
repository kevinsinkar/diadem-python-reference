---
title: "IRepCoordinateLabelAdditionalInt.XPositionOffset"
description: "Specifies the horizontal displacement of the coordinate labels as a percentage in a 2D or 3D axis system in the Coordinate display mode in DIAdem REPORT."
---

# IRepCoordinateLabelAdditionalInt.XPositionOffset

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XPositionOffset for AdditionalCoordinateLabel

Specifies the horizontal displacement of the coordinate labels as a percentage in a 2D or 3D axis system in the Coordinate display mode in DIAdem REPORT.

## Signature

```python
obj.XPositionOffset
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

oMyShape.XCoordinate.Reference = MaxValX
oMyShape.YCoordinate.Reference = MaxValY

oMyCoordLabel = oMyShape.Extensions.CoordinateLabel
oMyCoordLabel.Type = dd.e2DLabelValue
oMyCoordLabel.UseXPositionOffset = True
oMyCoordLabel.UseYPositionOffset = True
oMyCoordLabel.XPositionOffset = 5
oMyCoordLabel.YPositionOffset = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_XPositionOffset_IRepCoordinateLabelAdditionalInt.htm`*
