---
title: "IRepD3CharacteristicDiagramHyperbolaAdditionalInt"
description: "The 3DAdditionalHyperbolaLines object provides the properties for a hyperbola display in a characteristic diagram in DIAdem REPORT. A hyperbola describes at whi"
---

# IRepD3CharacteristicDiagramHyperbolaAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAdditionalHyperbolaLines

The 3DAdditionalHyperbolaLines object provides the properties for a hyperbola display in a characteristic diagram in DIAdem REPORT. A hyperbola describes at which points the product of x-values and y-values is the same.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-calculationtype/">CalculationType</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-font/">Font</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-format/">Format</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-gradationmanual/">GradationManual</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-gradationtype/">GradationType</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-insideboundary/">InsideBoundary</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-line/">Line</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-manualfactor/">ManualFactor</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-manualtargetunit/">ManualTargetUnit</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-unitbasedtargetunit/">UnitBasedTargetUnit</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-visible/">Visible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjcharacteristicdiagramextensionsint/">3DCharacteristicDiagramExtensions</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-hyperbola/">Hyperbola</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3CharacteristicDiagramHyperbolaAdditionalInt.htm`*
