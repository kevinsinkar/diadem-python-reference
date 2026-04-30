---
title: "IRepD3ShapeObjCharacteristicDiagramExtensionsInt.MeanMarkers"
description: "Specifies the mean values of the tolerance bands, in a characteristic diagram in DIAdem REPORT."
---

# IRepD3ShapeObjCharacteristicDiagramExtensionsInt.MeanMarkers

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MeanMarkers for 3DCharacteristicDiagramExtensions

Specifies the mean values of the tolerance bands, in a characteristic diagram in DIAdem REPORT.

## Signature

```python
return_value = obj.MeanMarkers
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.TripletStructure = dd.e3DCharacteristicTripletStructurePartialLoad
oMyPartialLoad = oMyShape.Settings.PartialLoad
oMyPartialLoad.PartialLoadToleranceType = dd.e3DPartialLoadToleranceAbsolute
oMyPartialLoad.AbsoluteTolerance = 3
oMy3DCurve.Shape.Extensions.MeanMarkers.Visible = True
oMyMeanMarkersLabel = oMy3DCurve.Shape.Extensions.MeanMarkers.Label
oMyMeanMarkersLabel.RelativePosition = dd.eRelativePositionCenter
oMyMeanMarkersLabel.Visible = True
oMyMeanMarkersLabel.RelativePosition = dd.eRelativePositionLeftTop
oMyMeanMarkersMarker = oMy3DCurve.Shape.Extensions.MeanMarkers.Marker
oMyMeanMarkersMarker.Type = dd.eMarkerCircle
oMyMeanMarkersMarker.Line.Width = dd.eLineWidth0050
oMyMeanMarkersMarker.Filling.ColorIndex = dd.eColorIndexDarkBlue
oMyMeanMarkersMarker.Size = 1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MeanMarkers_IRepD3ShapeObjCharacteristicDiagramExtensionsInt.htm`*
