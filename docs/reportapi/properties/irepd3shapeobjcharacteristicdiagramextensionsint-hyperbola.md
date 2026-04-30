---
title: "IRepD3ShapeObjCharacteristicDiagramExtensionsInt.Hyperbola"
description: "Specifies the display of hyperbolas in a characteristic diagram in DIAdem REPORT. Assign the value TRUE to the Visible property so that DIAdem REPORT displays t"
---

# IRepD3ShapeObjCharacteristicDiagramExtensionsInt.Hyperbola

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Hyperbola for 3DCharacteristicDiagramExtensions

Specifies the display of hyperbolas in a characteristic diagram in DIAdem REPORT. Assign the value TRUE to the Visible property so that DIAdem REPORT displays the hyperbolas.

## Signature

```python
return_value = obj.Hyperbola
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\" + "engine_characteristic_map","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.ZChannel.Reference = "[1]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
oMyShape.Extensions.Isoline.Visible = False
oMyHyperbola = oMy3DCurve.Shape.Extensions.Hyperbola
oMyHyperbola.Visible = True
oMyHyperbola.CalculationType = dd.e3DHyperbolaCalculationManual
oMyHyperbola.ManualTargetUnit = "W"
oMyHyperbola.ManualFactor = 2
oMyHyperbola.GradationType = dd.e3DHyperbolaGradationManual
oMyHyperbola.GradationManual = 200000
oMyHyperbola.Font.Size = 6
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Hyperbola_IRepD3ShapeObjCharacteristicDiagramExtensionsInt.htm`*
