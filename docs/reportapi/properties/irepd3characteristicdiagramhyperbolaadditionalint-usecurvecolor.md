---
title: "IRepD3CharacteristicDiagramHyperbolaAdditionalInt.UseCurveColor"
description: "Specifies whether DIAdem REPORT also uses the line color of the hyperbolas for the labels of the hyperbolas. Assign the value TRUE to the Visible property so th"
---

# IRepD3CharacteristicDiagramHyperbolaAdditionalInt.UseCurveColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCurveColor for 3DAdditionalHyperbolaLines

Specifies whether DIAdem REPORT also uses the line color of the hyperbolas for the labels of the hyperbolas. Assign the value TRUE to the Visible property so that DIAdem REPORT displays the hyperbolas.

## Signature

```python
obj.UseCurveColor
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
oMyHyperbola.UseCurveColor = False
oMyHyperbolaFont = oMyHyperbola.Font
oMyHyperbolaFont.Color.ColorIndex = dd.eColorIndexBlue
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCurveColor_IRepD3CharacteristicDiagramHyperbolaAdditionalInt.htm`*
