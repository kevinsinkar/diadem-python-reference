---
title: "IRepLineFullFeaturedInt"
description: "The FullFeaturedLine object provides the properties of a line in DIAdem REPORT."
---

# IRepLineFullFeaturedInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: FullFeaturedLine

The FullFeaturedLine object provides the properties of a line in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireplinefullfeaturedint-color/">Color</a> | <a href="../../properties/ireplinefullfeaturedint-interval/">Interval</a> | <a href="../../properties/ireplinefullfeaturedint-linetype/">LineType</a> | <a href="../../properties/ireplinefullfeaturedint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2specialcombadditionalstylesint/">2DAdditionalStyles</a>.<a href="../../properties/irepd2specialcombadditionalstylesint-line/">Line</a> | <a href="../irepd2shapeobjbarshorizontalsettingsint/">2DBarsHorizontalSettings</a>.<a href="../../properties/irepd2shapeobjbarshorizontalsettingsint-borderline/">BorderLine</a> | <a href="../irepd2shapeobjbarssettingsint/">2DBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarssettingsint-borderline/">BorderLine</a> | <a href="../irepd2shapeobjboxwhiskersettingsint/">2DBoxWhiskerSettings</a>.<a href="../../properties/irepd2shapeobjboxwhiskersettingsint-borderline/">BorderLine</a> | <a href="../irepd2shapeobjconstantsettingsint/">2DConstantSettings</a>.<a href="../../properties/irepd2shapeobjconstantsettingsint-line/">Line</a> | <a href="../irepd2shapeobjcoordinateextensionsint/">2DCoordinateExtensions</a>.<a href="../../properties/irepd2shapeobjcoordinateextensionsint-xconstantline/">XConstantLine</a> | <a href="../irepd2shapeobjcoordinateextensionsint/">2DCoordinateExtensions</a>.<a href="../../properties/irepd2shapeobjcoordinateextensionsint-yconstantline/">YConstantLine</a> | <a href="../irepd2shapeobjdifferentialsettingsint/">2DDifferentialSettings</a>.<a href="../../properties/irepd2shapeobjdifferentialsettingsint-borderline/">BorderLine</a> | <a href="../irepd2shapeobjfilledareasettingsint/">2DFilledAreaSettings</a>.<a href="../../properties/irepd2shapeobjfilledareasettingsint-line/">Line</a> | <a href="../irepd2shapeobjbarsgroupedsettingsint/">2DGroupedBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-borderline/">BorderLine</a> | <a href="../irepd2shapeobjlineandpointssettingsint/">2DLineAndPointsSettings</a>.<a href="../../properties/irepd2shapeobjlineandpointssettingsint-line/">Line</a> | <a href="../irepd2shapeobjlinesettingsint/">2DLineSettings</a>.<a href="../../properties/irepd2shapeobjlinesettingsint-line/">Line</a> | <a href="../irepd2shapeobjoutlbarshorizontalsettingsint/">2DOutlineBarsHorizontalSettings</a>.<a href="../../properties/irepd2shapeobjoutlbarshorizontalsettingsint-line/">Line</a> | <a href="../irepd2shapeobjoutlbarssettingsint/">2DOutlineBarsSettings</a>.<a href="../../properties/irepd2shapeobjoutlbarssettingsint-line/">Line</a> | <a href="../irepd2shapeobjspecialcombinationsettingsint/">2DSpecialCombinationSettings</a>.<a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-line/">Line</a> | <a href="../irepd2shapeobjspikeshorizontalsettingsint/">2DSpikesHorizontalSettings</a>.<a href="../../properties/irepd2shapeobjspikeshorizontalsettingsint-line/">Line</a> | <a href="../irepd2shapeobjspikessettingsint/">2DSpikesSettings</a>.<a href="../../properties/irepd2shapeobjspikessettingsint-line/">Line</a> | <a href="../irepd2shapeobjbarsstackedsettingsint/">2DStackedBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarsstackedsettingsint-borderline/">BorderLine</a> | <a href="../irepd3boundarycurveadditionalint/">3DAdditionalBoundaryCurve</a>.<a href="../../properties/irepd3boundarycurveadditionalint-line/">Line</a> | <a href="../irepd3characteristicdiagramisolineadditionalint/">3DAdditionalCharacteristicDiagramIsoline</a>.<a href="../../properties/irepd3characteristicdiagramisolineadditionalint-line/">Line</a> | <a href="../irepd3characteristicdiagramhyperbolaadditionalint/">3DAdditionalHyperbolaLines</a>.<a href="../../properties/irepd3characteristicdiagramhyperbolaadditionalint-line/">Line</a> | <a href="../irepd3additionalisolineint/">3DAdditionalIsoline</a>.<a href="../../properties/irepd3additionalisolineint-line/">Line</a> | <a href="../irepd3surfaceisolineadditionalint/">3DAdditionalSurfaceIsoline</a>.<a href="../../properties/irepd3surfaceisolineadditionalint-line/">Line</a> | <a href="../irepd3shapeobjbarssettingsint/">3DBarsSettings</a>.<a href="../../properties/irepd3shapeobjbarssettingsint-line/">Line</a> | <a href="../irepd3shapeobjisolinessettingsint/">3DIsolinesSettings</a>.<a href="../../properties/irepd3shapeobjisolinessettingsint-line/">Line</a> | <a href="../irepd3shapeobjlinesettingsint/">3DLineSettings</a>.<a href="../../properties/irepd3shapeobjlinesettingsint-line/">Line</a> | <a href="../irepd3shapeobjmatrix2dsettingsint/">3DMatrix2DSettings</a>.<a href="../../properties/irepd3shapeobjmatrix2dsettingsint-line/">Line</a> | <a href="../../collections/3dpalettecoloredlines/">3DPaletteColoredLines</a>.<a href="../../methods/irepd3palettecoloredlinelistint-item/">Item</a> | <a href="../irepd3planegridxyint/">3DPlaneGridXY</a>.<a href="../../properties/irepd3planegridxyint-linex/">LineX</a> | <a href="../irepd3planegridxyint/">3DPlaneGridXY</a>.<a href="../../properties/irepd3planegridxyint-liney/">LineY</a> | <a href="../irepd3planegridxzint/">3DPlaneGridXZ</a>.<a href="../../properties/irepd3planegridxzint-linex/">LineX</a> | <a href="../irepd3planegridxzint/">3DPlaneGridXZ</a>.<a href="../../properties/irepd3planegridxzint-linez/">LineZ</a> | <a href="../irepd3planegridyzint/">3DPlaneGridYZ</a>.<a href="../../properties/irepd3planegridyzint-liney/">LineY</a> | <a href="../irepd3planegridyzint/">3DPlaneGridYZ</a>.<a href="../../properties/irepd3planegridyzint-linez/">LineZ</a> | <a href="../irepd3planexyint/">3DPlaneXY</a>.<a href="../../properties/irepd3planexyint-borderline/">BorderLine</a> | <a href="../irepd3planexzint/">3DPlaneXZ</a>.<a href="../../properties/irepd3planexzint-borderline/">BorderLine</a> | <a href="../irepd3planeyzint/">3DPlaneYZ</a>.<a href="../../properties/irepd3planeyzint-borderline/">BorderLine</a> | <a href="../irepd3shapeobjspikesettingsint/">3DSpikesSettings</a>.<a href="../../properties/irepd3shapeobjspikesettingsint-line/">Line</a> | <a href="../irepd3shapeobjsurfacesettingsint/">3DSurfaceSettings</a>.<a href="../../properties/irepd3shapeobjsurfacesettingsint-line/">Line</a> | <a href="../irepd3shapeobjvectorsettingsint/">3DVectorSettings</a>.<a href="../../properties/irepd3shapeobjvectorsettingsint-line/">Line</a> | <a href="../irepd3shapeobjwaterfallsettingsint/">3DWaterfallSettings</a>.<a href="../../properties/irepd3shapeobjwaterfallsettingsint-line/">Line</a> | <a href="../ireppolarshapeobjdifferentialint/">PolarDifferential</a>.<a href="../../properties/ireppolarshapeobjdifferentialint-differentialline/">DifferentialLine</a> | <a href="../ireppolarradialaxisint/">PolarRadialAxis</a>.<a href="../../properties/ireppolarradialaxisint-minitickline/">MiniTickLine</a> | <a href="../ireppolarradialaxisint/">PolarRadialAxis</a>.<a href="../../properties/ireppolarradialaxisint-tickline/">TickLine</a> | <a href="../ireppolarsectorsint/">PolarSectors</a>.<a href="../../properties/ireppolarsectorsint-minisectorline/">MiniSectorLine</a> | <a href="../ireppolarsectorsint/">PolarSectors</a>.<a href="../../properties/ireppolarsectorsint-sectorline/">SectorLine</a> | <a href="../ireppolarshapeobjspikesint/">PolarSpike</a>.<a href="../../properties/ireppolarshapeobjspikesint-spike/">Spike</a> | <a href="../irepspidershapeobjlineandpointssettingsint/">SpiderLineAndPointsSettings</a>.<a href="../../properties/irepspidershapeobjlineandpointssettingsint-line/">Line</a> | <a href="../irepspidershapeobjlinesettingsint/">SpiderLineSettings</a>.<a href="../../properties/irepspidershapeobjlinesettingsint-line/">Line</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLineFullFeaturedInt.htm`*
