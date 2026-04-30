---
title: "IRepD3ShapeObjCharacteristicDiagramExtensionsInt"
description: "The 3DCharacteristicDiagramExtensions object provides the extended properties of the curve parameters of a 3D axis system in the Characteristic diagram display "
---

# IRepD3ShapeObjCharacteristicDiagramExtensionsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DCharacteristicDiagramExtensions

The 3DCharacteristicDiagramExtensions object provides the extended properties of the curve parameters of a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT.

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
oMyShape.DataStructure = dd.e3DDataStructureMatrix
iChannelMax = dd.Data.Root.ChannelGroups(2).Channels(3).Properties("maximum").Value
iChannelMin = dd.Data.Root.ChannelGroups(2).Channels(3).Properties("minimum").Value
oMyIsoValTable = oMyShape.Settings.IsoValueTable
oMyIsoValTable.Count = 5
oMy3DCurve.Shape.Extensions.Isoline.Type = dd.e3DCharacteristicIsoValueFromIsoValueTable
oMy3DCurve.Shape.Extensions.Isoline.Color.ColorIndex = dd.eColorIndexPalette
for i in range( 1, oMyIsoValTable.Count+1):
    oMyIsoValTable.Item(i).Color.SetPredefinedColor(i)
    oMyIsoValTable.Item(i).Interval = 20
    oMyIsoValTable.Item(i).LineType = dd.eLineTypeDotted
    oMyIsoValTable.Item(i).UpperLimit = iChannelMin + (iChannelMax - iChannelMin) / oMyIsoValTable.Count * i
    oMyIsoValTable.Item(i).Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-additionalisolines/">AdditionalIsolines</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-boundarycurve/">BoundaryCurve</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-boundarypoints/">BoundaryPoints</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-hyperbola/">Hyperbola</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-invalidvalues/">InvalidValues</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-isoline/">Isoline</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-maximumpoint/">MaximumPoint</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-meanmarkers/">MeanMarkers</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-measurementpoints/">MeasurementPoints</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramextensionsint-minimumpoint/">MinimumPoint</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjcharacteristicdiagramint/">3DCharacteristicDiagram</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramint-extensions/">Extensions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjCharacteristicDiagramExtensionsInt.htm`*
