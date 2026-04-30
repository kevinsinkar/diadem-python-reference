---
title: "IToBirdsEyeViewChartInt.DoubleBuffered"
description: "Specifies whether DIAdem plots without flickers while refreshing a bird's eye view display in DIAdem VIEW."
---

# IToBirdsEyeViewChartInt.DoubleBuffered

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DoubleBuffered for BirdsEyeView

Specifies whether DIAdem plots without flickers while refreshing a bird's eye view display in DIAdem VIEW.

## Signature

```python
obj.DoubleBuffered
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem uses two buffers when plotting graphics. DIAdem displays the contents of the first buffer and plots the graphic into the second buffer that is in the background. When DIAdem has finished plotting the graphic, DIAdem exchanges the buffers. Because exchanging the buffers occurs faster than the plotting, DIAdem can ensure that the plotting is flicker free. Therefore, DIAdem refreshes the display after the plotting process is complete. When plotting a lot of data, it may seem that DIAdem is not reacting. When you are working interactively and want to display long channels, use the setting <span class="Monospace">DoubleBuffered = FALSE</span>. When programming events, use the setting <span class="Monospace">DoubleBuffered = TRUE</span>.</td></tr></table>
</div>

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMySheet.ActiveArea.DisplayObj.DoubleBuffered = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DoubleBuffered_IToBirdsEyeViewChartInt.htm`*
