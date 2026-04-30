---
title: "IRepD3ShapeObjCharacteristicDiagramSettingsInt.PartialLoad"
description: "Specifies a partial load structure in a characteristic diagram in DIAdem REPORT."
---

# IRepD3ShapeObjCharacteristicDiagramSettingsInt.PartialLoad

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PartialLoad for 3DCharacteristicDiagramSettings

Specifies a partial load structure in a characteristic diagram in DIAdem REPORT.

## Signature

```python
return_value = obj.PartialLoad
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
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.TripletStructure = dd.e3DCharacteristicTripletStructurePartialLoad
oMyPartialLoad = oMyShape.Settings.PartialLoad
oMyPartialLoad.PartialLoadToleranceType = dd.e3DPartialLoadToleranceAbsolute
oMyPartialLoad.AbsoluteTolerance = 3
oMyPartialLoad.ShowToleranceBand = True
oMyPartialLoad.MinNumberOfPoints = 5
oMyPartialLoad.CheckZValue = True
oMyPartialLoad.MinimumZValue = -1
oMyPartialLoad.MaximumZValue = 0.5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PartialLoad_IRepD3ShapeObjCharacteristicDiagramSettingsInt.htm`*
