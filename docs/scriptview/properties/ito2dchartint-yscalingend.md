---
title: "ITo2DChartInt.YScalingEnd"
description: "Specifies the greatest value of the y-scaling of a 2D axis system in DIAdem VIEW if manual scaling is set. DIAdem includes this setting only if the YScalingMode"
---

# ITo2DChartInt.YScalingEnd

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: YScalingEnd for CurveChart2D

Specifies the greatest value of the y-scaling of a 2D axis system in DIAdem VIEW if manual scaling is set. DIAdem includes this setting only if the YScalingMode property contains the value manual .

## Signature

```python
obj.YScalingEnd
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "CurveChart2D"
oMyChart = dd.View.Sheets(1).Areas(1).DisplayObj
oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMyChart.YScaling = "1 system [phys.]"
oMyChart.YScalingMode = "manual"
oMyChart.YScalingBegin = 0
oMyChart.YScalingEnd = 10
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Analyzing and Displaying Channels Section by Section</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Background Segments in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Show texts of assignment channels in the VIEW legend</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_YScalingEnd_ITo2DChartInt.htm`*
