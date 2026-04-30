---
title: "IRepLineEndLabelAdditionalInt.UseLabelOnlyOnFirstExpandedCurve"
description: "Specifies whether DIAdem REPORT only uses curve end labels for the first curve in 2D axis systems with expanding curves in the display modes Line and points or "
---

# IRepLineEndLabelAdditionalInt.UseLabelOnlyOnFirstExpandedCurve

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseLabelOnlyOnFirstExpandedCurve for AdditionalLineEndLabel

Specifies whether DIAdem REPORT only uses curve end labels for the first curve in 2D axis systems with expanding curves in the display modes Line and points or Special combination .

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
oMyAttributeList = oMyCurveExpansion.AttributeList
oMyAttributeList.Enable = True
oMyExpansionLineStyle = oMyAttributeList.LineStyles
oMyAttributeList.UseLineInterval = True
oMyAttributeList.UseLineType = True
oMyAttributeList.UseLineWidth = True
oMyAttributeList.UseMarkerProperties = True
oMyAttributeList.UseMarkerType = True
for I in range( 1, oMyExpansionLineStyle.Count+1):
    oMyExpansionLineStyle(I).Line.Width = dd.eLineWidth0070
    oMyExpansionLineStyle(I).Line.LineType = dd.eLineTypeDashDot
    oMyExpansionLineStyle(I).Line.Interval = 5
    oMyExpansionLineStyle(I).Marker.Size = 3
    oMyExpansionLineStyle(I).Marker.Type = dd.eMarkerCircle
    oMyExpansionLineStyle(I).Marker.RepetitionMode = dd.eMarkerRepetitionMaximalNPoints
    oMyExpansionLineStyle(I).Marker.MarkerPointCount = 20
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.Settings.UseCurveExpansion = True
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"
oMyEndLabel = oMyCurve.Shape.Extensions.EndLabel
oMyEndLabel.UseLabelOnlyOnFirstExpandedCurve = True
oMyEndLabel.Position = dd.e2DLineEndLabelPositionLargestXValue
oMyEndLabel.Type = dd.e2DLineEndLabelCustomText
oMyEndLabel.Text = "End label"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseLabelOnlyOnFirstExpandedCurve_IRepLineEndLabelAdditionalInt.htm`*
