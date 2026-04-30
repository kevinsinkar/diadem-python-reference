---
title: "IRepD3CharacteristicDiagramHyperbolaAdditionalInt.Font"
description: "Specifies the properties of the hyperbola label in a characteristic diagram in DIAdem REPORT. Assign the value TRUE to the Visible property so that DIAdem REPOR"
---

# IRepD3CharacteristicDiagramHyperbolaAdditionalInt.Font

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Font for 3DAdditionalHyperbolaLines

Specifies the properties of the hyperbola label in a characteristic diagram in DIAdem REPORT. Assign the value TRUE to the Visible property so that DIAdem REPORT displays the hyperbolas.

## Signature

```python
return_value = obj.Font
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
oMyHyperbolaFont = oMyHyperbola.Font
oMyHyperbolaFont.Size = 3
oMyHyperbolaFont.Bold = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Font_IRepD3CharacteristicDiagramHyperbolaAdditionalInt.htm`*
