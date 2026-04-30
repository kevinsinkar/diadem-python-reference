---
title: "IRepCommentPositionAdditionalInt"
description: "The AdditionalCommentPosition object provides the position of an additional comment in the 2D and 3D display mode Coordinate in DIAdem REPORT."
---

# IRepCommentPositionAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AdditionalCommentPosition

The AdditionalCommentPosition object provides the position of an additional comment in the 2D and 3D display mode Coordinate in DIAdem REPORT.

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
oMyCoordShape.BoundingType = dd.eCoordinateChannelBounded
oMyCoordShape.BoundingPosition = dd.e2DCoordinateBoundingAbsoluteMax
oMyCoordShape.BoundingXChannel.Reference = "[1]/[1]"
oMyCoordShape.BoundingyChannel.Reference = "[1]/[2]"

oMyCoordShape.Settings.Type = dd.eMarkerCircle
oMyCoordComment = oMyCoordShape.Extensions.CoordinateComment
oMyCoordCommArrow = oMyCoordComment.Arrow
oMyCoordCommArrow.SymbolBegin = dd.eArrowHeadPoint
oMyCoordCommArrow.SymbolEnd = dd.eArrowHeadStandardArrow
oMyCoordCommArrow.Line.LineType = dd.eLineTypeSolid
oMyCoordShape.Settings.Size = 2
oMyCoordShape.Settings.MarkerFilling.SetPredefinedColor(dd.eColorIndexDarkBlue)

MaxValY = dd.Data.GetChannel("[1]/[2]").Properties("maximum").Value
MaxValX = dd.Data.GetChannel("[1]/[1]").Values(dd.PNo("[1]/[2]", MaxValY))
oMyCoordShape.XCoordinate.Reference = MaxValX
oMyCoordShape.YCoordinate.Reference = MaxValY
oMyCoordComment.Visible = True
oMyCoordCommPosition = oMyCoordComment.Position
oMyCoordCommPosition.OffsetX = 20
oMyCoordCommPosition.OffsetY = 10
oMyCoordCommPosition.Width = 25
oMyCoordCommPosition.Height = 8

oMyCoordComment.Comment.Text = "Max. X: " + MaxValX + "\r\n" + "Max. Y: " + MaxValY
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcommentpositionadditionalint-height/">Height</a> | <a href="../../properties/irepcommentpositionadditionalint-offsetx/">OffsetX</a> | <a href="../../properties/irepcommentpositionadditionalint-offsety/">OffsetY</a> | <a href="../../properties/irepcommentpositionadditionalint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcommentadditionalint/">AdditionalComment</a>.<a href="../../properties/irepcommentadditionalint-position/">Position</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCommentPositionAdditionalInt.htm`*
