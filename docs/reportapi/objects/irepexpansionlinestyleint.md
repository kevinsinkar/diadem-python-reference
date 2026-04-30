---
title: "IRepExpansionLineStyleInt"
description: "The ExpansionLineStyle object provides the line and marker properties of an expanding curve in DIAdem REPORT."
---

# IRepExpansionLineStyleInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ExpansionLineStyle

The ExpansionLineStyle object provides the line and marker properties of an expanding curve in DIAdem REPORT.

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.Settings.UseCurveExpansion = True
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepexpansionlinestyleint-line/">Line</a> | <a href="../../properties/irepexpansionlinestyleint-marker/">Marker</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/expansionlinestyles/">ExpansionLineStyles</a>.<a href="../../methods/irepexpansionlinestylelistint-add/">Add</a> | <a href="../../collections/expansionlinestyles/">ExpansionLineStyles</a>.<a href="../../methods/irepexpansionlinestylelistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepExpansionLineStyleInt.htm`*
