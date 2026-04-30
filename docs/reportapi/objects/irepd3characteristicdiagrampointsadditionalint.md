---
title: "IRepD3CharacteristicDiagramPointsAdditionalInt"
description: "The 3DAdditionalCharacteristicDiagramPoints object provides the properties of the boundary curve points, the maximum and the minimum, and the measuring points o"
---

# IRepD3CharacteristicDiagramPointsAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAdditionalCharacteristicDiagramPoints

The 3DAdditionalCharacteristicDiagramPoints object provides the properties of the boundary curve points, the maximum and the minimum, and the measuring points of a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\engine_characteristic_map.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.ZChannel.Reference = "[1]/[3]"
oMyShape.Extensions.BoundaryCurve.Visible = True
oMyShape.Extensions.BoundaryPoints.Visible = True
oMyLabel = oMyShape.Extensions.BoundaryPoints.Label
oMyLabel.Visible = True
oMyLabel.Font.Size = 4
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3characteristicdiagrampointsadditionalint-label/">Label</a> | <a href="../../properties/irepd3characteristicdiagrampointsadditionalint-marker/">Markers</a> | <a href="../../properties/irepd3characteristicdiagrampointsadditionalint-usedatareductionvalues/">UseDataReductionValues</a> | <a href="../../properties/irepd3characteristicdiagrampointsadditionalint-visible/">Visible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjcharacteristicdiagramextensionsint/">3DCharacteristicDiagramExtensions</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-boundarypoints/">BoundaryPoints</a> | <a href="../irepd3shapeobjcharacteristicdiagramextensionsint/">3DCharacteristicDiagramExtensions</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-invalidvalues/">InvalidValues</a> | <a href="../irepd3shapeobjcharacteristicdiagramextensionsint/">3DCharacteristicDiagramExtensions</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-maximumpoint/">MaximumPoint</a> | <a href="../irepd3shapeobjcharacteristicdiagramextensionsint/">3DCharacteristicDiagramExtensions</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-meanmarkers/">MeanMarkers</a> | <a href="../irepd3shapeobjcharacteristicdiagramextensionsint/">3DCharacteristicDiagramExtensions</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-measurementpoints/">MeasurementPoints</a> | <a href="../irepd3shapeobjcharacteristicdiagramextensionsint/">3DCharacteristicDiagramExtensions</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-minimumpoint/">MinimumPoint</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3CharacteristicDiagramPointsAdditionalInt.htm`*
