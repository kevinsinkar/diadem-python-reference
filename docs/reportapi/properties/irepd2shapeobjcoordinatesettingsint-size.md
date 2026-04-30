---
title: "IRepD2ShapeObjCoordinateSettingsInt.Size"
description: "Specifies the size of the marker symbols as a percentage of the worksheet in the Coordinate display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjCoordinateSettingsInt.Size

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Size for 2DCoordinateSettings

Specifies the size of the marker symbols as a percentage of the worksheet in the Coordinate display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Size
```

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
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue" contenteditable="false">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMy2DAxisSystem, oMyCurveLine, oMyPos, oMyShape, oMyCurveCoord, oMyCoordShape, oMyCoordComment, MaxValX, MaxValY
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.NewLayout</span>()
<span class="HlVBSKeyword">Set</span> oMy2DAxisSystem = <span class="Hldiademobject">Report.ActiveSheet.Objects.Add</span>(<span class="Hldiademconstant">eReportObject2DAxisSystem</span>,<span class="HlString">"My2DAxisSystem"</span>)
<span class="HlVBSKeyword">Set</span> oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(<span class="Hldiademconstant">e2DShapeLine</span>,<span class="HlString">"My2DCurveLine"</span>)
<span class="HlVBSKeyword">Set</span> oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = <span class="HlNumbers">20</span>
oMyPos.X2 = <span class="HlNumbers">80</span>
oMyPos.Y1 = <span class="HlNumbers">20</span>
oMyPos.Y2 = <span class="HlNumbers">80</span>
<span class="HlVBSKeyword">Set</span> oMyShape = oMyCurveLine.Shape
oMyShape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span> 
oMyShape.YChannel.Reference = <span class="HlString">"[1]/[2]"</span>
<span class="HlVBSKeyword">Set</span> oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(<span class="Hldiademconstant">e2DShapeCoordinate</span>,<span class="HlString">"My2DCurveCoord"</span>)
MaxValY = <span class="Hldiademobject">Data.GetChannel</span>(<span class="HlString">"[1]/[2]"</span>).Properties(<span class="HlString">"maximum"</span>).Value
MaxValX = <span class="Hldiademobject">Data.GetChannel</span>(<span class="HlString">"[1]/[1]"</span>).Values(<span class="Hldiademcommand"><span class="Hldiademcommand">PNo</span></span>(<span class="HlString">"[1]/[2]"</span>, MaxValY))
<span class="HlVBSKeyword">Set</span> oMyCoordShape = oMyCurveCoord.Shape
oMyCoordShape.BoundingType = <span class="Hldiademconstant">eCoordinateChannelBounded</span>
oMyCoordShape.BoundingPosition =<span class="Hldiademconstant">e2DCoordinateBoundingAbsoluteMax</span> 
oMyCoordShape.BoundingXChannel.Reference = <span class="HlString">"[1]/[1]"</span>
oMyCoordShape.BoundingyChannel.Reference = <span class="HlString">"[1]/[2]"</span>
<span class="HlVBSKeyword">Set</span> oMyCoordComment = oMyCoordShape.Extensions.CoordinateComment
oMyCoordShape.Settings.Type = <span class="Hldiademconstant">eMarkerCircle</span>
oMyCoordComment.Arrow.SymbolBegin = <span class="Hldiademconstant">eArrowHeadPoint</span>
oMyCoordComment.Arrow.SymbolEnd = <span class="Hldiademconstant">eArrowHeadStandardArrow</span>
oMyCoordComment.Arrow.Line.LineType = <span class="Hldiademconstant">eLineTypeSolid</span>
oMyCoordShape.Settings.Size = <span class="HlNumbers">2</span>
<span class="HlVBSKeyword">Call</span> oMyCoordShape.Settings.MarkerFilling.SetPredefinedColor(<span class="Hldiademconstant">eColorIndexDarkBlue</span>)
oMyCoordShape.XCoordinate.Reference = MaxValX
oMyCoordShape.YCoordinate.Reference = MaxValY
oMyCoordComment.Visible = <span class="HlVBSKeyword">True</span>
oMyCoordComment.Position.OffsetX = <span class="HlNumbers">20</span>
oMyCoordComment.Position.OffsetY = <span class="HlNumbers">10</span>
oMyCoordComment.Position.Width = <span class="HlNumbers">25</span>
oMyCoordComment.Position.Height = <span class="HlNumbers">8</span>
oMyCoordComment.Comment.Text = <span class="HlString">"Max. X: "</span> &amp; MaxValX &amp; <span class="HlVBSKeyword">vbCrLf</span> &amp; <span class="HlString">"Max. Y: "</span> &amp; MaxValY
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.Refresh</span>()</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.Report.NewLayout() 
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,<span class="HlString">"My2DAxisSystem"</span>) 
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,<span class="HlString">"My2DCurveLine"</span>) 
oMyPos = oMy2DAxisSystem.Position.ByCoordinate 
oMyPos.X1 = <span class="HlNumbers">20</span> 
oMyPos.X2 = <span class="HlNumbers">80</span> 
oMyPos.Y1 = <span class="HlNumbers">20</span> 
oMyPos.Y2 = <span class="HlNumbers">80</span> 
oMyShape = oMyCurveLine.Shape 
oMyShape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span> 
oMyShape.YChannel.Reference = <span class="HlString">"[1]/[2]"</span> 
oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,<span class="HlString">"My2DCurveCoord"</span>) 
MaxValY = dd.Data.GetChannel(<span class="HlString">"[1]/[2]"</span>).Properties(<span class="HlString">"maximum"</span>).Value 
MaxValX = dd.Data.GetChannel(<span class="HlString">"[1]/[1]"</span>).Values(dd.PNo(<span class="HlString">"[1]/[2]"</span>, MaxValY)) 
oMyCoordShape = oMyCurveCoord.Shape 
oMyCoordShape.BoundingType = dd.eCoordinateChannelBounded 
oMyCoordShape.BoundingPosition =dd.e2DCoordinateBoundingAbsoluteMax 
oMyCoordShape.BoundingXChannel.Reference = <span class="HlString">"[1]/[1]"</span> 
oMyCoordShape.BoundingyChannel.Reference = <span class="HlString">"[1]/[2]"</span> 
oMyCoordComment = oMyCoordShape.Extensions.CoordinateComment 
oMyCoordShape.Settings.Type = dd.eMarkerCircle 
oMyCoordComment.Arrow.SymbolBegin = dd.eArrowHeadPoint 
oMyCoordComment.Arrow.SymbolEnd = dd.eArrowHeadStandardArrow 
oMyCoordComment.Arrow.Line.LineType = dd.eLineTypeSolid 
oMyCoordShape.Settings.Size = <span class="HlNumbers">2</span> 
oMyCoordShape.Settings.MarkerFilling.SetPredefinedColor(dd.eColorIndexDarkBlue) 
oMyCoordShape.XCoordinate.Reference = MaxValX 
oMyCoordShape.YCoordinate.Reference = MaxValY 
oMyCoordComment.Visible = <span class="HlVBSKeyword">True</span> 
oMyCoordComment.Position.OffsetX = <span class="HlNumbers">20</span> 
oMyCoordComment.Position.OffsetY = <span class="HlNumbers">10</span> 
oMyCoordComment.Position.Width = <span class="HlNumbers">25</span> 
oMyCoordComment.Position.Height = <span class="HlNumbers">8</span> 
oMyCoordComment.Comment.Text = <span class="HlString">"Max. X: "</span> + MaxValX + <span class="HlString">"\r\n"</span> + <span class="HlString">"Max. Y: "</span> + MaxValY 
dd.Report.Refresh() 
	 
</donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Size_IRepD2ShapeObjCoordinateSettingsInt.htm`*
