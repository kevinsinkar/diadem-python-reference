---
title: "ITo2DChartInt"
description: "The CurveChart2D object provides a 2D axis system in DIAdem VIEW."
---

# ITo2DChartInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: CurveChart2D

The CurveChart2D object provides a 2D axis system in DIAdem VIEW.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyCurve = oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ito2dchartint-abscissa/">Abscissa</a> | <a href="../../properties/ito2dchartint-area/">Area</a> | <a href="../../properties/ito2dchartint-axislabeling/">AxisLabeling</a> | <a href="../../properties/ito2dchartint-constants/">Constants</a> | <a href="../../properties/ito2dchartint-curves2d/">Curves2D</a> | <a href="../../properties/ito2dchartint-datetimerepresentation/">DateTimeRepresentation</a> | <a href="../../properties/ito2dchartint-decorations/">Decorations</a> | <a href="../../properties/ito2dchartint-doublebuffered/">DoubleBuffered</a> | <a href="../../properties/ito2dchartint-lastzoommode/">LastZoomMode</a> | <a href="../../properties/ito2dchartint-legenditems/">LegendItems</a> | <a href="../../properties/ito2dchartint-legendwidth/">LegendWidth</a> | <a href="../../properties/ito2dchartint-ordinate/">Ordinate</a> | <a href="../../properties/ito2dchartint-segments/">Segments</a> | <a href="../../properties/ito2dchartint-sound/">Sound</a> | <a href="../../properties/ito2dchartint-subcursor/">SubCursor</a> | <a href="../../properties/ito2dchartint-subcursortype/">SubCursorType</a> | <a href="../../properties/ito2dchartint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/ito2dchartint-usecurverelatedyscaling/">UseCurveRelatedYScaling</a> | <a href="../../properties/ito2dchartint-xaxismargin/">XAxisMargin</a> | <a href="../../properties/ito2dchartint-xaxismarginmode/">XAxisMarginMode</a> | <a href="../../properties/ito2dchartint-xbegin/">XBegin</a> | <a href="../../properties/ito2dchartint-xend/">XEnd</a> | <a href="../../properties/ito2dchartint-xscalingmode/">XScalingMode</a> | <a href="../../properties/ito2dchartint-xscalingtype/">XScalingType</a> | <a href="../../properties/ito2dchartint-yaxismargin/">YAxisMargin</a> | <a href="../../properties/ito2dchartint-yaxismarginmode/">YAxisMarginMode</a> | <a href="../../properties/ito2dchartint-ybegin/">YBegin</a> | <a href="../../properties/ito2dchartint-yend/">YEnd</a> | <a href="../../properties/ito2dchartint-yscaling/">YScaling</a> | <a href="../../properties/ito2dchartint-yscalingbegin/">YScalingBegin</a> | <a href="../../properties/ito2dchartint-yscalingend/">YScalingEnd</a> | <a href="../../properties/ito2dchartint-yscalinglist/">YScalingList</a> | <a href="../../properties/ito2dchartint-yscalingmode/">YScalingMode</a> | <a href="../../properties/ito2dchartint-zoomcursor/">ZoomCursor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ito2dchartint-setzoom/">SetZoom</a> | <a href="../../methods/ito2dchartint-showcurvesdlg/">ShowCurvesDlg</a> | <a href="../../methods/ito2dchartint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itoareaobjectint/">Area</a>.<a href="../../properties/itoareaobjectint-displayobj/">DisplayObj</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Analyzing and Displaying Channels Section by Section</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Background Segments in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Show texts of assignment channels in the VIEW legend</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_ITo2DChartInt.htm`*
