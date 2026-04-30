---
title: "IRepCoordinateLabelAdditionalInt.UseLabelOnlyOnFirstExpandedCurve"
description: "Specifies whether DIAdem REPORT only labels the first curve in 2D and 3D axis systems with expanding curves in the Coordinate display mode."
---

# IRepCoordinateLabelAdditionalInt.UseLabelOnlyOnFirstExpandedCurve

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseLabelOnlyOnFirstExpandedCurve for AdditionalCoordinateLabel

Specifies whether DIAdem REPORT only labels the first curve in 2D and 3D axis systems with expanding curves in the Coordinate display mode.

## Signature

```python
obj.UseLabelOnlyOnFirstExpandedCurve
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "TR_M17_QT_32-1.tdm","TDM","")
dd.Report.NewLayout()
oMyReportSettings = dd.Report.Settings
oMyCurveExpansion = oMyReportSettings.CurveExpansion
oMyCurveExpansion.Enable = True
oMyCurveExpansion.Mode = dd.eCurveExpansionModeSortByChannels
oMyAttributeList = oMyCurveExpansion.AttributeList
oMyAttributeList.Enable = True
oMyAttributeList.UseLineInterval = True
oMyAttributeList.UseLineType = True
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurveLine")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyShape = oMyCurveLine.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"
oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,"My2DCurveCoord")
MaxValY = dd.Data.Root.ChannelGroups(1).Channels("Temp_A").Properties("maximum").Value
MaxValX = dd.ChDWfX(dd.PNo("Temp_A", MaxValY),1)
oMyCoordShape = oMyCurveCoord.Shape
oMyCoordShape.BoundingType = dd.eCoordinateChannelBounded
oMyCoordShape.BoundingPosition =dd.e2DCoordinateBoundingAbsoluteMax
oMyCoordShape.BoundingXChannel.Reference = ""
oMyCoordShape.BoundingyChannel.Reference = "Temp_A"
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
oMyCoordComment.Position.OffsetY = 5
oMyCoordComment.Position.Width = 25
oMyCoordComment.Position.Height = 6
oMyCoordComment.Comment.Text = "X: @@str(CurrXValue,\"AutoAdj\")@@" + "\r\n" + "Y: @@str(CurrYValue,\"AutoAdj\")@@"
oMyCoordLabel = oMyCoordShape.Extensions.CoordinateLabel
oMyCoordLabel.UseLabelOnlyOnFirstExpandedCurve = True
oMyCoordLabel.Type = dd.eEndLabelCoordinate
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

*Source: `ReportApi/properties/Report_property_UseLabelOnlyOnFirstExpandedCurve_IRepCoordinateLabelAdditionalInt.htm`*
