---
title: "IRepD2PaletteInt"
description: "The 2DPalette object provides the properties of the palette in 2D axis systems or in polar axis systems in DIAdem REPORT."
---

# IRepD2PaletteInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DPalette

The 2DPalette object provides the properties of the palette in 2D axis systems or in polar axis systems in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyReportObj = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMyReportObj.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyReportObj.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
iChannelMax = dd.Data.Root.ChannelGroups(1).Channels(2).Properties("maximum").Value
iChannelMin = dd.Data.Root.ChannelGroups(1).Channels(2).Properties("minimum").Value
oMyLine = oMyShape.Settings.Line
oMyLine.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyShape.Settings.Palette.Lines
i = 0
for oMyPaletteLine in oMyPalette:
    i = i + 1
    oMyPaletteLine.LineType = dd.eLineTypeDashDot
    oMyPaletteLine.Interval = 10
    oMyPaletteLine.Width = dd.eLineWidth0035
    oMyPaletteLine.UpperLimit = iChannelMin + (iChannelMax - iChannelMin) / oMyPalette.Count * i
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2paletteint-beginvalue/">BeginValue</a> | <a href="../../properties/irepd2paletteint-channel/">Channel</a> | <a href="../../properties/irepd2paletteint-endvalue/">EndValue</a> | <a href="../../properties/irepd2paletteint-lines/">Lines</a> | <a href="../../properties/irepd2paletteint-valuetype/">ValueType</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjbarshorizontalsettingsint/">2DBarsHorizontalSettings</a>.<a href="../../properties/irepd2shapeobjbarshorizontalsettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjbarssettingsint/">2DBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarssettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjconstantsettingsint/">2DConstantSettings</a>.<a href="../../properties/irepd2shapeobjconstantsettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjcoordinatesettingsint/">2DCoordinateSettings</a>.<a href="../../properties/irepd2shapeobjcoordinatesettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjdifferentialsettingsint/">2DDifferentialSettings</a>.<a href="../../properties/irepd2shapeobjdifferentialsettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjfilledareasettingsint/">2DFilledAreaSettings</a>.<a href="../../properties/irepd2shapeobjfilledareasettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjlineandpointssettingsint/">2DLineAndPointsSettings</a>.<a href="../../properties/irepd2shapeobjlineandpointssettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjlinesettingsint/">2DLineSettings</a>.<a href="../../properties/irepd2shapeobjlinesettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjoutlbarshorizontalsettingsint/">2DOutlineBarsHorizontalSettings</a>.<a href="../../properties/irepd2shapeobjoutlbarshorizontalsettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjoutlbarssettingsint/">2DOutlineBarsSettings</a>.<a href="../../properties/irepd2shapeobjoutlbarssettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjspecialcombinationsettingsint/">2DSpecialCombinationSettings</a>.<a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjspikeshorizontalsettingsint/">2DSpikesHorizontalSettings</a>.<a href="../../properties/irepd2shapeobjspikeshorizontalsettingsint-palette/">Palette</a> | <a href="../irepd2shapeobjspikessettingsint/">2DSpikesSettings</a>.<a href="../../properties/irepd2shapeobjspikessettingsint-palette/">Palette</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2PaletteInt.htm`*
