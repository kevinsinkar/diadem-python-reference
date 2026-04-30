---
title: "IToCascadeChartInt"
description: "The Cascade object provides a cascade display in DIAdem VIEW. Use the Cascade object to display a waterfall and an order line and to define the display."
---

# IToCascadeChartInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Cascade

The Cascade object provides a cascade display in DIAdem VIEW. Use the Cascade object to display a waterfall and an order line and to define the display.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\cascade.tdm","TDM","")
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Cascade"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.CurvesCascade.AddCascade("[2]/[1]","[2]/[2]","[2]/[3]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itocascadechartint-area/">Area</a> | <a href="../../properties/itocascadechartint-axislabeling/">AxisLabeling</a> | <a href="../../properties/itocascadechartint-createdynamicorderline/">CreateDynamicOrderLine</a> | <a href="../../properties/itocascadechartint-cursorsynchronisationabscissa/">CursorSynchronisationAbscissa</a> | <a href="../../properties/itocascadechartint-cursorsynchronisationordinate/">CursorSynchronisationOrdinate</a> | <a href="../../properties/itocascadechartint-cursorsynchronisationz/">CursorSynchronisationZ</a> | <a href="../../properties/itocascadechartint-curvescascade/">CurvesCascade</a> | <a href="../../properties/itocascadechartint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/itocascadechartint-doublebuffered/">DoubleBuffered</a> | <a href="../../properties/itocascadechartint-inclinationanglehorizontal/">InclinationAngleHorizontal</a> | <a href="../../properties/itocascadechartint-inclinationanglevertical/">InclinationAngleVertical</a> | <a href="../../properties/itocascadechartint-legenditems/">LegendItems</a> | <a href="../../properties/itocascadechartint-legendwidth/">LegendWidth</a> | <a href="../../properties/itocascadechartint-showdynamicorderline/">ShowDynamicOrderLine</a> | <a href="../../properties/itocascadechartint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itocascadechartint-xaxismargin/">XAxisMargin</a> | <a href="../../properties/itocascadechartint-xaxismarginmode/">XAxisMarginMode</a> | <a href="../../properties/itocascadechartint-xbegin/">XBegin</a> | <a href="../../properties/itocascadechartint-xend/">XEnd</a> | <a href="../../properties/itocascadechartint-xscalingtype/">XScalingType</a> | <a href="../../properties/itocascadechartint-yaxismargin/">YAxisMargin</a> | <a href="../../properties/itocascadechartint-yaxismarginmode/">YAxisMarginMode</a> | <a href="../../properties/itocascadechartint-ybegin/">YBegin</a> | <a href="../../properties/itocascadechartint-yend/">YEnd</a> | <a href="../../properties/itocascadechartint-yscalingbegin/">YScalingBegin</a> | <a href="../../properties/itocascadechartint-yscalingend/">YScalingEnd</a> | <a href="../../properties/itocascadechartint-yscalingmode/">YScalingMode</a> | <a href="../../properties/itocascadechartint-yscalingtype/">YScalingType</a> | <a href="../../properties/itocascadechartint-zbegin/">ZBegin</a> | <a href="../../properties/itocascadechartint-zend/">ZEnd</a> | <a href="../../properties/itocascadechartint-zlabelchannelname/">ZLabelChannelName</a> | <a href="../../properties/itocascadechartint-zoomcursor/">ZoomCursor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itocascadechartint-iszoomed/">IsZoomed</a> | <a href="../../methods/itocascadechartint-showcurvesdlg/">ShowCurvesDlg</a> | <a href="../../methods/itocascadechartint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itoareaobjectint/">Area</a>.<a href="../../properties/itoareaobjectint-displayobj/">DisplayObj</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToCascadeChartInt.htm`*
