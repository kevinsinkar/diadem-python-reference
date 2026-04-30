---
title: "IRepPaletteLineColorInt"
description: "The PaletteColor object provides the colors of a color palette in DIAdem REPORT."
---

# IRepPaletteLineColorInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PaletteColor

The PaletteColor object provides the colors of a color palette in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")

oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeGroupedBars, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = ""
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.Settings.DisplayMode = dd.eBarsDisplayMode2D
oMy2DCurve.Shape.Settings.Filling.Color.ColorIndex = dd.eColorIndexPalette
oMy2DCurve.Shape.Settings.BorderLine.Color.ColorIndex = dd.eColorIndexPalette

oMyPaletteColors = oMy2DCurve.Shape.Settings.Palette.Colors
oMyPaletteColors(1).ColorIndex = dd.eColorIndexDarkYellow
oMyPaletteColors(2).ColorIndex = dd.eColorIndexBlue
oMyPaletteColors(1).Transparency = 10

oMy2DCurve.Shape.Settings.Filling.Pattern = dd.eFillPatternLeftDiagonal

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppalettelinecolorint-colorindex/">ColorIndex</a> | <a href="../../properties/ireppalettelinecolorint-gradientdirection/">GradientDirection</a> | <a href="../../properties/ireppalettelinecolorint-gradientmode/">GradientMode</a> | <a href="../../properties/ireppalettelinecolorint-rgb/">RGB</a> | <a href="../../properties/ireppalettelinecolorint-rgbfilling/">RGBFilling</a> | <a href="../../properties/ireppalettelinecolorint-transparency/">Transparency</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireppalettelinecolorint-setfillingcolor/">SetFillingColor</a> | <a href="../../methods/ireppalettelinecolorint-setpredefinedcolor/">SetPredefinedColor</a> | <a href="../../methods/ireppalettelinecolorint-setrgbcolor/">SetRGBColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisgridint/">2DAxisGrid</a>.<a href="../../properties/irepd2axisgridint-color/">Color</a> | <a href="../irepd2axisminitickgridint/">2DAxisMiniTick</a>.<a href="../../properties/irepd2axisminitickgridint-color/">Color</a> | <a href="../irepd2segmentint/">2DBackgroundSegment</a>.<a href="../../properties/irepd2segmentint-color/">Color</a> | <a href="../irepd2barfillingint/">2DBarFilling</a>.<a href="../../properties/irepd2barfillingint-color/">Color</a> | <a href="../irepboxwhiskerfillingint/">2DBoxWhiskerFilling</a>.<a href="../../properties/irepboxwhiskerfillingint-color/">Color</a> | <a href="../irepboxwhiskerlineint/">2DBoxWhiskerLine</a>.<a href="../../properties/irepboxwhiskerlineint-color/">Color</a> | <a href="../irepboxwhiskermarkerlineint/">2DBoxWhiskerMarkerLine</a>.<a href="../../properties/irepboxwhiskermarkerlineint-color/">Color</a> | <a href="../irepd2shapeobjconstantsettingsint/">2DConstantSettings</a>.<a href="../../properties/irepd2shapeobjconstantsettingsint-xfillingcolor/">XFillingColor</a> | <a href="../irepd2shapeobjconstantsettingsint/">2DConstantSettings</a>.<a href="../../properties/irepd2shapeobjconstantsettingsint-xyfillingcolor/">XYFillingColor</a> | <a href="../irepd2shapeobjconstantsettingsint/">2DConstantSettings</a>.<a href="../../properties/irepd2shapeobjconstantsettingsint-yfillingcolor/">YFillingColor</a> | <a href="../irepd2shapeobjcoordinateextensionsint/">2DCoordinateExtensions</a>.<a href="../../properties/irepd2shapeobjcoordinateextensionsint-xfillingcolor/">XFillingColor</a> | <a href="../irepd2shapeobjcoordinateextensionsint/">2DCoordinateExtensions</a>.<a href="../../properties/irepd2shapeobjcoordinateextensionsint-xyfillingcolor/">XYFillingColor</a> | <a href="../irepd2shapeobjcoordinateextensionsint/">2DCoordinateExtensions</a>.<a href="../../properties/irepd2shapeobjcoordinateextensionsint-yfillingcolor/">YFillingColor</a> | <a href="../irepd2errorbarlineint/">2DErrorBarLine</a>.<a href="../../properties/irepd2errorbarlineint-color/">Color</a> | <a href="../ireptable2dgridlineint/">2DTableGridLine</a>.<a href="../../properties/ireptable2dgridlineint-color/">Color</a> | <a href="../ireptable2dsettingsint/">2DTableSettings</a>.<a href="../../properties/ireptable2dsettingsint-borderlinecolor/">BorderLineColor</a> | <a href="../irepd3spikesadditionalint/">3DAdditionalSpikes</a>.<a href="../../properties/irepd3spikesadditionalint-color/">Color</a> | <a href="../irepd3vectorcurveadditionalint/">3DAdditionalVectorCurve</a>.<a href="../../properties/irepd3vectorcurveadditionalint-color/">Color</a> | <a href="../irepd3barfillingint/">3DBarFilling</a>.<a href="../../properties/irepd3barfillingint-edgecolor/">EdgeColor</a> | <a href="../irepd3isovaluetableitemint/">3DIsoValueTableItem</a>.<a href="../../properties/irepd3isovaluetableitemint-color/">Color</a> | <a href="../irepd3shapeobjsurfacesettingsint/">3DSurfaceSettings</a>.<a href="../../properties/irepd3shapeobjsurfacesettingsint-additionalgridcolor/">AdditionalGridColor</a> | <a href="../irepd3shapeobjsurfacesettingsint/">3DSurfaceSettings</a>.<a href="../../properties/irepd3shapeobjsurfacesettingsint-lowersurfacecolor/">LowerSurfaceColor</a> | <a href="../ireptable3dsettingsint/">3DTableSettings</a>.<a href="../../properties/ireptable3dsettingsint-linecolor/">LineColor</a> | <a href="../ireparrowlineint/">ArrowLine</a>.<a href="../../properties/ireparrowlineint-color/">Color</a> | <a href="../irepaxislineint/">AxisLine</a>.<a href="../../properties/irepaxislineint-color/">Color</a> | <a href="../irepborderlineint/">BorderLine</a>.<a href="../../properties/irepborderlineint-color/">Color</a> | <a href="../irepcurveexpansionlineint/">CurveExpansionLine</a>.<a href="../../properties/irepcurveexpansionlineint-color/">Color</a> | <a href="../irepfilleffectsint/">FillEffects</a>.<a href="../../properties/irepfilleffectsint-color/">Color</a> | <a href="../irepfontint/">Font</a>.<a href="../../properties/irepfontint-color/">Color</a> | <a href="../irepfontborderedint/">FontWithBorder</a>.<a href="../../properties/irepfontborderedint-color/">Color</a> | <a href="../irepformuladisplayint/">FormulaDisplay</a>.<a href="../../properties/irepformuladisplayint-fontcolor/">FontColor</a> | <a href="../irepframelineint/">FrameLine</a>.<a href="../../properties/irepframelineint-color/">Color</a> | <a href="../ireplinefullfeaturedint/">FullFeaturedLine</a>.<a href="../../properties/ireplinefullfeaturedint-color/">Color</a> | <a href="../ireplegendframeint/">LegendFrame</a>.<a href="../../properties/ireplegendframeint-color/">Color</a> | <a href="../irepmarkerlineint/">MarkerLine</a>.<a href="../../properties/irepmarkerlineint-color/">Color</a> | <a href="../../collections/palettecolors/">PaletteColors</a>.<a href="../../methods/ireppalettelinecolorlistint-item/">Item</a> | <a href="../ireppalettelineint/">PaletteLine</a>.<a href="../../properties/ireppalettelineint-color/">Color</a> | <a href="../ireppiechartsliceint/">PieChartSlice</a>.<a href="../../properties/ireppiechartsliceint-filleffects/">FillEffects</a> | <a href="../ireppolarlineint/">PolarCurveLine</a>.<a href="../../properties/ireppolarlineint-color/">Color</a> | <a href="../irepshadowint/">Shadow</a>.<a href="../../properties/irepshadowint-color/">Color</a> | <a href="../irepsolidlineint/">SolidLine</a>.<a href="../../properties/irepsolidlineint-color/">Color</a> | <a href="../ireppalettecolorint/">TablePaletteColor</a>.<a href="../../properties/ireppalettecolorint-color/">Color</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPaletteLineColorInt.htm`*
