---
title: "IRepCommentArrowAdditionalInt.SymbolBegin"
description: "Specifies the type of arrowhead which DIAdem REPORT plots at the beginning of a comment arrow in the 2D display mode Coordinate ."
---

# IRepCommentArrowAdditionalInt.SymbolBegin

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SymbolBegin for AdditionalCommentArrow

Specifies the type of arrowhead which DIAdem REPORT plots at the beginning of a comment arrow in the 2D display mode Coordinate .

## Signature

```python
obj.SymbolBegin
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eArrowHeadNone` | 0 | No arrow |
| `eArrowHeadStandardArrow` | 1 | Standard arrow |
| `eArrowHeadNormArrow` | 2 | Norm arrow |
| `eArrowHeadPoint` | 3 | Arrow with point |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurveLine")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyShape = oMyCurveLine.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,"My2DCurveCoord")
MaxValY = dd.Data.GetChannel("[1]/[2]").Properties("maximum").Value
MaxValX = dd.Data.GetChannel("[1]/[1]").Values(dd.PNo("[1]/[2]", MaxValY))
oMyCoordShape = oMyCurveCoord.Shape
oMyCoordShape.BoundingType = dd.eCoordinateChannelBounded
oMyCoordShape.BoundingPosition =dd.e2DCoordinateBoundingAbsoluteMax
oMyCoordShape.BoundingXChannel.Reference = "[1]/[1]"
oMyCoordShape.BoundingyChannel.Reference = "[1]/[2]"
oMyCoordComment = oMyCoordShape.Extensions.CoordinateComment
oMyCoordShape.Settings.Type = dd.eMarkerCircle
oMyCoordComment.Arrow.SymbolBegin = dd.eArrowHeadPoint
oMyCoordComment.Arrow.SymbolEnd = dd.eArrowHeadStandardArrow
oMyCoordComment.Arrow.Line.LineType = dd.eLineTypeSolid
oMyCoordShape.Settings.Size = 2
oMyCoordShape.Settings.MarkerFilling.SetPredefinedColor(dd.eColorIndexDarkBlue)
oMyCoordShape.XCoordinate.Reference = MaxValX
oMyCoordShape.YCoordinate.Reference = MaxValY
oMyCoordComment.Visible = True
oMyCoordComment.Position.OffsetX = 20
oMyCoordComment.Position.OffsetY = 10
oMyCoordComment.Position.Width = 25
oMyCoordComment.Position.Height = 8
oMyCoordComment.Comment.Text = "Max. X: " + MaxValX + "\r\n" + "Max. Y: " + MaxValY
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SymbolBegin_IRepCommentArrowAdditionalInt.htm`*
