---
title: "IToPolarChartInt.DoubleBuffered"
description: "Specifies whether DIAdem plots a polar axis system without flickers during the update in DIAdem VIEW."
---

# IToPolarChartInt.DoubleBuffered

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DoubleBuffered for Polar

Specifies whether DIAdem plots a polar axis system without flickers during the update in DIAdem VIEW.

## Signature

```python
obj.DoubleBuffered
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>DIAdem uses two buffers when plotting graphics. DIAdem displays the contents of the first buffer and plots the graphic into the second buffer that is in the background. When DIAdem has finished plotting the graphic, DIAdem exchanges the buffers. Because exchanging the buffers occurs faster than the plotting, DIAdem can ensure that the plotting is flicker free. Therefore DIAdem refreshes the display after the plotting process is complete. When a lot of data must be plotted, it might seem that DIAdem is not reacting. When you are working interactively in VIEW and want to display long channels, use the setting  <span class="Monospace">DoubleBuffered = FALSE</span>. When you program events, use the setting <span class="Monospace">DoubleBuffered = TRUE</span>.</td></tr></table>
</div>

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "Polar"
oMyChart = dd.View.Sheets(1).Areas(1).DisplayObj
oMyChart.CurvesPolar.Add("[1]/[1]","[1]/[3]")
oMyChart.DoubleBuffered = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DoubleBuffered_IToPolarChartInt.htm`*
