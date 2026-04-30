---
title: "IRepCoordinateMarkerFillingInt.SetPredefinedColor"
description: "Assigns a pre-defined color to a marker of an additional comment, which DIAdem REPORT uses in 2D or 3D axis systems in the Coordinate display mode. The method a"
---

# IRepCoordinateMarkerFillingInt.SetPredefinedColor

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetPredefinedColor for CoordinateMarkerFilling

Assigns a pre-defined color to a marker of an additional comment, which DIAdem REPORT uses in 2D or 3D axis systems in the Coordinate display mode. The method also specifies the Color object properties which are necessary to display the predefined colors.

## Signature

```python
obj.SetPredefinedColor(Value)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorIndexNone` | 0 | None |
| `eColorIndexBlack` | 1 | Black |
| `eColorIndexRed` | 2 | Red |
| `eColorIndexGreen` | 3 | Green |
| `eColorIndexBlue` | 4 | Blue |
| `eColorIndexViolet` | 5 | Violet |
| `eColorIndexTurquoise` | 6 | Turquoise |
| `eColorIndexGrey` | 7 | Gray |
| `eColorIndexYellow` | 8 | Yellow |
| `eColorIndexDarkRed` | 9 | Dark red |
| `eColorIndexDarkGreen` | 10 | Dark green |
| `eColorIndexDarkBlue` | 11 | Dark blue |
| `eColorIndexDarkViolet` | 12 | Dark violet |
| `eColorIndexDarkTurquoise` | 13 | Dark turquoise |
| `eColorIndexDarkGrey` | 14 | Dark gray |
| `eColorIndexDarkYellow` | 15 | Dark yellow |
| `eColorIndexWhite` | 16 | White |

## Python example

```python
sXChannel =  "[1]/[1]"
sYChannel =  "[1]/[2]"
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurveLine")
oMyCurveShape = oMyCurveLine.Shape
oMyCurveShape.XChannel.Reference = sXChannel
oMyCurveShape.YChannel.Reference = sYChannel

oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,"My2DCurveCoord")
oMyCoordShape = oMyCurveCoord.Shape
oMyCoordShape.BoundingType = dd.eCoordinateChannelBounded
oMyCoordShape.BoundingPosition = dd.e2DCoordinateBoundingAbsoluteMax
oMyCoordShape.BoundingXChannel.Reference = sXChannel
oMyCoordShape.BoundingyChannel.Reference = sYChannel

oMyCoordShape.Settings.Type = dd.eMarkerCircle
oMyCoordComment = oMyCoordShape.Extensions.CoordinateComment
oMyCoordCommArrow = oMyCoordComment.Arrow
oMyCoordCommArrow.SymbolBegin = dd.eArrowHeadPoint
oMyCoordCommArrow.SymbolEnd = dd.eArrowHeadStandardArrow
oMyCoordCommArrow.Line.LineType = dd.eLineTypeSolid
oMyCoordShape.Settings.Size = 2
oMyCoordShape.Settings.MarkerFilling.UseMarkerColor = False
oMyCoordShape.Settings.MarkerFilling.SetPredefinedColor(dd.eColorIndexDarkBlue)

MaxValY = dd.Data.GetChannel(sYChannel).Properties("maximum").Value
MaxValX = dd.Data.GetChannel(sXChannel).Values(dd.PNo(sYChannel, MaxValY))
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetPredefinedColor_IRepCoordinateMarkerFillingInt.htm`*
