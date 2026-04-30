---
title: "IRepD3ShapeObjCharacteristicDiagramExtensionsInt.InvalidValues"
description: "Specifies the invalid value of a partial load structure in a characteristic diagram in DIAdem REPORT. You must assign the value e3DCharacteristicTripletStructur"
---

# IRepD3ShapeObjCharacteristicDiagramExtensionsInt.InvalidValues

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: InvalidValues for 3DCharacteristicDiagramExtensions

Specifies the invalid value of a partial load structure in a characteristic diagram in DIAdem REPORT. You must assign the value e3DCharacteristicTripletStructurePartialLoad to the TripletStructure property so that you can use the InvalidValues property. You must also assign the value True to the Visible property so that DIAdem displays the invalid values.

## Signature

```python
return_value = obj.InvalidValues
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
oMy3DCurve.Shape.Extensions.InvalidValues.Visible = True
oMyInvalidValueLabel = oMy3DCurve.Shape.Extensions.InvalidValues.Label
oMyInvalidValueLabel.RelativePosition = dd.eRelativePositionCenter
oMyInvalidValueLabel.Visible = True
oMyInvalidValueLabel.RelativePosition = dd.eRelativePositionLeftTop
oMyInvalidValueMarker = oMy3DCurve.Shape.Extensions.InvalidValues.Marker
oMyInvalidValueMarker.Type = dd.eMarkerCircle
oMyInvalidValueMarker.Line.Width = dd.eLineWidth0050
oMyInvalidValueMarker.Filling.ColorIndex = dd.eColorIndexYellow
oMyInvalidValueMarker.Size = 1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_InvalidValues_IRepD3ShapeObjCharacteristicDiagramExtensionsInt.htm`*
