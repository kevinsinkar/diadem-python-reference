---
title: "IRepCommentPositionAdditionalInt.OffsetY"
description: "Specifies in DIAdem REPORT the vertical distance, in centimeters or inches, between the comment in the Coordinate 2D display mode and the origin of the axis sys"
---

# IRepCommentPositionAdditionalInt.OffsetY

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OffsetY for AdditionalCommentPosition

Specifies in DIAdem REPORT the vertical distance, in centimeters or inches, between the comment in the Coordinate 2D display mode and the origin of the axis system, as a percentage of the worksheet.

## Signature

```python
obj.OffsetY
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
oMyCurveShape = oMyCurveLine.Shape
oMyCurveShape.XChannel.Reference = "[1]/[1]"
oMyCurveShape.YChannel.Reference = "[1]/[2]"
oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,"My2DCurveCoord")
oMyCoordShape = oMyCurveCoord.Shape
oMyCoordShape.BoundingType = dd.eCoordinateFree
MaxValY = dd.Data.GetChannel("[1]/[2]").Properties("maximum").Value
MaxValX = dd.Data.GetChannel("[1]/[1]").Values(dd.PNo("[1]/[2]", MaxValY))
oMyCoordShape.XCoordinate.Reference = MaxValX
oMyCoordShape.YCoordinate.Reference = MaxValY

oMyCoordShape.Settings.Type = dd.eMarkerCircle
oMyCoordShape.Settings.MarkerFilling.SetPredefinedColor(dd.eColorIndexDarkBlue)

oMyCoordComment = oMyCoordShape.Extensions.CoordinateComment
oMyCoordComment.Visible = True
oMyCoordCommPosition = oMyCoordComment.Position
oMyCoordCommPosition.OffsetX = 20
oMyCoordCommPosition.OffsetY = 10
oMyCoordCommPosition.Width = 25
oMyCoordCommPosition.Height = 8
oMyCoordComment.Comment.Text = "Max. X: " + MaxValX + "\r\n" + "Max. Y: " + MaxValY

oMyCoordCommArrow = oMyCoordComment.Arrow
oMyCoordCommArrow.SymbolBegin = dd.eArrowHeadPoint
oMyCoordCommArrow.SymbolEnd = dd.eArrowHeadStandardArrow
oMyCoordCommArrow.Line.LineType = dd.eLineTypeSolid
oMyCoordShape.Settings.Size = 2

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OffsetY_IRepCommentPositionAdditionalInt.htm`*
