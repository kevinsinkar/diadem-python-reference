---
title: "3DPaletteColoredLines"
description: "The 3DPaletteColoredLines object provides the color palette properties of a 3D axis system in DIAdem REPORT."
---

# 3DPaletteColoredLines

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 3DPaletteColoredLines

The 3DPaletteColoredLines object provides the color palette properties of a 3D axis system in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.Extensions.SurfaceIsoline.DisplayType = dd.e3DIsolineCorrespondingToIsoValueAndProjected
oMyShape.Extensions.SurfaceIsoline.Visible = True
oMyShape.Extensions.SurfaceIsoline.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColoredLines = oMyShape.Settings.Palette
for i in range( 1, oMyColoredLines.Count+1):
    oMyColoredLines(i).LineType = dd.eLineTypeDashDot
    oMyColoredLines(i).Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3palettecoloredlinelistint-channel/">Channel</a> | <a href="../../properties/irepd3palettecoloredlinelistint-count/">Count</a> | <a href="../../properties/irepd3palettecoloredlinelistint-valuetype/">ValueType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd3palettecoloredlinelistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd3shapeobjbarssettingsint/">3DBarsSettings</a>.<a href="../../properties/irepd3shapeobjbarssettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjcharacteristicdiagramsettingsint/">3DCharacteristicDiagramSettings</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjcoordinatesettingsint/">3DCoordinateSettings</a>.<a href="../../properties/irepd3shapeobjcoordinatesettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjisolinessettingsint/">3DIsolinesSettings</a>.<a href="../../properties/irepd3shapeobjisolinessettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjlinesettingsint/">3DLineSettings</a>.<a href="../../properties/irepd3shapeobjlinesettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjmatrix2dsettingsint/">3DMatrix2DSettings</a>.<a href="../../properties/irepd3shapeobjmatrix2dsettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjpointssettingsint/">3DPointsSettings</a>.<a href="../../properties/irepd3shapeobjpointssettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjspikesettingsint/">3DSpikesSettings</a>.<a href="../../properties/irepd3shapeobjspikesettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjsurfacesettingsint/">3DSurfaceSettings</a>.<a href="../../properties/irepd3shapeobjsurfacesettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjvectorsettingsint/">3DVectorSettings</a>.<a href="../../properties/irepd3shapeobjvectorsettingsint-palette/">Palette</a> | <a href="../../objects/irepd3shapeobjwaterfallsettingsint/">3DWaterfallSettings</a>.<a href="../../properties/irepd3shapeobjwaterfallsettingsint-palette/">Palette</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3PaletteColoredLineListInt.htm`*
