---
title: "IRepExpansionMarkerInt.MinimumDisplaySize"
description: "Specifies the minimum size of the markers at which DIAdem starts drawing additional markers of expanding curves in DIAdem REPORT."
---

# IRepExpansionMarkerInt.MinimumDisplaySize

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MinimumDisplaySize for CurveExpansionMarker

Specifies the minimum size of the markers at which DIAdem starts drawing additional markers of expanding curves in DIAdem REPORT.

## Signature

```python
obj.MinimumDisplaySize
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
oMyAttributeList.UseMarkerProperties = True
oMyAttributeList.UseMarkerType = True
for I in range( 1, oMyExpansionLineStyle.Count+1):
    oMyExpansionLineStyle(I).Marker.MinimumDisplaySize = 3
    oMyExpansionLineStyle(I).Marker.Channel.Reference = "[1]/[1]"
    oMyExpansionLineStyle(I).Marker.Type = dd.eMarkerCircle
    oMyExpansionLineStyle(I).Marker.RepetitionMode = dd.eMarkerRepetitionMaximalNPoints
    oMyExpansionLineStyle(I).Marker.MarkerPointCount = 20

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.Settings.UseCurveExpansion = True
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MinimumDisplaySize_IRepExpansionMarkerInt.htm`*
