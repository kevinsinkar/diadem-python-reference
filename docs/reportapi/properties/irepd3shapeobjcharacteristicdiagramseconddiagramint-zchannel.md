---
title: "IRepD3ShapeObjCharacteristicDiagramSecondDiagramInt.ZChannel"
description: "Specifies the z-channel of the differential characteristic diagram in a Characteristic diagram display in a 3D axis system in DIAdem REPORT."
---

# IRepD3ShapeObjCharacteristicDiagramSecondDiagramInt.ZChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ZChannel for 3DCharacteristicDiagramSecondDiagram

Specifies the z-channel of the differential characteristic diagram in a Characteristic diagram display in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.ZChannel
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
oMyShape.Type = dd.e3DCharacteristicDifferential
oMyShape.DifferentialType = dd.e3DCharacteristicDifferentialRelative
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMySecondDiagram = oMyShape.SecondDiagram
oMySecondDiagram.XChannel.Reference = "[3]/[1]"
oMySecondDiagram.YChannel.Reference = "[3]/[2]"
oMySecondDiagram.ZChannel.Reference = "[3]/[3]"
oMySecondDiagram.DataStructure = dd.e3DDataStructureTriplet
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ZChannel_IRepD3ShapeObjCharacteristicDiagramSecondDiagramInt.htm`*
