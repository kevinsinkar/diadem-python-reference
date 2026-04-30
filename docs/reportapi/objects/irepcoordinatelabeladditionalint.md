---
title: "IRepCoordinateLabelAdditionalInt"
description: "The AdditionalCoordinateLabel object provides the properties of the coordinate labels in 2D and 3D axis systems in the Coordinate display mode in DIAdem REPORT."
---

# IRepCoordinateLabelAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AdditionalCoordinateLabel

The AdditionalCoordinateLabel object provides the properties of the coordinate labels in 2D and 3D axis systems in the Coordinate display mode in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcoordinatelabeladditionalint-angle/">Angle</a> | <a href="../../properties/irepcoordinatelabeladditionalint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepcoordinatelabeladditionalint-font/">Font</a> | <a href="../../properties/irepcoordinatelabeladditionalint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepcoordinatelabeladditionalint-text/">Text</a> | <a href="../../properties/irepcoordinatelabeladditionalint-type/">Type</a> | <a href="../../properties/irepcoordinatelabeladditionalint-uselabelonlyonfirstexpandedcurve/">UseLabelOnlyOnFirstExpandedCurve</a> | <a href="../../properties/irepcoordinatelabeladditionalint-usemarkercolor/">UseMarkerColor</a> | <a href="../../properties/irepcoordinatelabeladditionalint-usexpositionoffset/">UseXPositionOffset</a> | <a href="../../properties/irepcoordinatelabeladditionalint-useypositionoffset/">UseYPositionOffset</a> | <a href="../../properties/irepcoordinatelabeladditionalint-xpositionoffset/">XPositionOffset</a> | <a href="../../properties/irepcoordinatelabeladditionalint-ypositionoffset/">YPositionOffset</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjcoordinateextensionsint/">2DCoordinateExtensions</a>.<a href="../../properties/irepd2shapeobjcoordinateextensionsint-coordinatelabel/">CoordinateLabel</a> | <a href="../irepd3shapeobjcoordinateextensionsint/">3DCoordinateExtensions</a>.<a href="../../properties/irepd3shapeobjcoordinateextensionsint-coordinatelabel/">CoordinateLabel</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCoordinateLabelAdditionalInt.htm`*
