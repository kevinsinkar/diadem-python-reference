---
title: "IRepD3ShapeObjCharacteristicDiagramInt.Extensions"
description: "Specifies the extended properties of a curve in the Characteristic diagram display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3ShapeObjCharacteristicDiagramInt.Extensions

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Extensions for 3DCharacteristicDiagram

Specifies the extended properties of a curve in the Characteristic diagram display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Extensions
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
oMyMaximumPoint = oMyShape.Extensions.MaximumPoint
oMyMaximumPoint.Visible = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Extensions_IRepD3ShapeObjCharacteristicDiagramInt.htm`*
