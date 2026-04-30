---
title: "IRepD3ShapeObjCharacteristicDiagramInt.TripletStructure"
description: "Specifies how triplet data is distributed in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT."
---

# IRepD3ShapeObjCharacteristicDiagramInt.TripletStructure

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TripletStructure for 3DCharacteristicDiagram

Specifies how triplet data is distributed in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT.

## Signature

```python
obj.TripletStructure
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.TripletStructure = dd.e3DCharacteristicTripletStructurePartialLoad
oMyShape.Settings.PartialLoadTolerance = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TripletStructure_IRepD3ShapeObjCharacteristicDiagramInt.htm`*
