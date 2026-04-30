---
title: "IRepD2ShapeObjCoordinateSettingsInt.Type"
description: "Specifies the symbol which DIAdem REPORT displays in a 2D axis system as curve marker in the Coordinate display mode."
---

# IRepD2ShapeObjCoordinateSettingsInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 2DCoordinateSettings

Specifies the symbol which DIAdem REPORT displays in a 2D axis system as curve marker in the Coordinate display mode.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eMarkerNone` | 0 | None |
| `eMarkerSquare` | 1 | Square |
| `eMarkerRhombus` | 2 | Rhombus |
| `eMarkerTriangle` | 3 | Triangle |
| `eMarkerCross` | 4 | Cross |
| `eMarkerAsterisk` | 5 | Asterisk |
| `eMarkerShortDash` | 6 | Short dash |
| `eMarkerLongDash` | 7 | Long dash |
| `eMarkerPlus` | 8 | Plus |
| `eMarkerCircle` | 9 | Circle |
| `eMarkerTriangle_Bottom` | 10 | Triangle bottom |
| `eMarkerTriangle_Left` | 11 | Triangle left |
| `eMarkerTriangle_Right` | 12 | Triangle right |
| `eMarkerSquare_Top` | 13 | Square filled top |
| `eMarkerSquare_Bottom` | 14 | Square filled bottom |
| `eMarkerSquare_Left` | 15 | Square filled left |
| `eMarkerSquare_Right` | 16 | Square filled right |
| `eMarkerRhomb_Top` | 17 | Rhomb filled top |
| `eMarkerRhomb_Bottom` | 18 | Rhomb filled bottom |
| `eMarkerRhomb_Left` | 19 | Rhomb filled left |
| `eMarkerRhomb_Right` | 20 | Rhomb filled right |
| `eMarkerTriangle1_Left` | 21 | Triangle 1 filled left |
| `eMarkerTriangle1_Right` | 22 | Triangle 1 filled right |
| `eMarkerTriangle2_Left` | 23 | Triangle 2 filled left |
| `eMarkerTriangle2_Right` | 24 | Triangle 2 filled right |
| `eMarkerTriangle3_Top` | 25 | Triangle 3 filled top |
| `eMarkerTriangle3_Bottom` | 26 | Triangle 3 filled bottom |
| `eMarkerTriangle4_Top` | 27 | Triangle 4 filled top |
| `eMarkerTriangle4_Bottom` | 28 | Triangle 4 filled bottom |

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

*Source: `ReportApi/properties/Report_property_Type_IRepD2ShapeObjCoordinateSettingsInt.htm`*
