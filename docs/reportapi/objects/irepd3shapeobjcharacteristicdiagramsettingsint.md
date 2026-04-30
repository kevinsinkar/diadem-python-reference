---
title: "IRepD3ShapeObjCharacteristicDiagramSettingsInt"
description: "The 3DCharacteristicDiagramSettings object provides the properties of the curve parameters of a 3D axis system in the Characteristic diagram display mode in DIA"
---

# IRepD3ShapeObjCharacteristicDiagramSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DCharacteristicDiagramSettings

The 3DCharacteristicDiagramSettings object provides the properties of the curve parameters of a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT.

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
<p><a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-colorlegend/">ColorLegend</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-interpolation/">Interpolation</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-isovaluetable/">IsoValueTable</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-palette/">Palette</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-partialload/">PartialLoad</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-showhiddenlines/">ShowHiddenLines</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-surfacecolortype/">SurfaceColorType</a> | <a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-visible/">Visible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjcharacteristicdiagramint/">3DCharacteristicDiagram</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjCharacteristicDiagramSettingsInt.htm`*
