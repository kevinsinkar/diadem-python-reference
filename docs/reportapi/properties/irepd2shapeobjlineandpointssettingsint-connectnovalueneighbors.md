---
title: "IRepD2ShapeObjLineAndPointsSettingsInt.ConnectNoValueNeighbors"
description: "Specifies whether DIAdem REPORT connects NoValues in curves in the Line and Points display mode in a 2D axis system."
---

# IRepD2ShapeObjLineAndPointsSettingsInt.ConnectNoValueNeighbors

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ConnectNoValueNeighbors for 2DLineAndPointsSettings

Specifies whether DIAdem REPORT connects NoValues in curves in the Line and Points display mode in a 2D axis system.

## Signature

```python
obj.ConnectNoValueNeighbors
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMySetting.ConnectNoValueNeighbors = True
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 3
oMyMarker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyMarker.Repetition.NValue = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ConnectNoValueNeighbors_IRepD2ShapeObjLineAndPointsSettingsInt.htm`*
