---
title: "IToChannelTableInt.CursorMode"
description: "Specifies whether DIAdem synchronizes the cursor and the channel table. If you enable synchronization and you idle a crosshair cursor over the curve point, DIAd"
---

# IToChannelTableInt.CursorMode

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: CursorMode for ChannelTable

Specifies whether DIAdem synchronizes the cursor and the channel table. If you enable synchronization and you idle a crosshair cursor over the curve point, DIAdem highlights the corresponding row in the channel table. If you enable synchronization and you idle a band or frame cursor over the curve point, DIAdem highlights the corresponding row range in the channel table.

## Signature

```python
obj.CursorMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eVIEWChannelTableCursorNone` | 0 | Do not synchronize with cursor |
| `eVIEWChannelTableHighlightRows` | 1 | Synchronize with cursor |

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyCurveChart = oMySheet.ActiveArea.DisplayObj
oMyCurveChart.Curves2D.Add ("[1]/[1]", "[1]/[2]")
oMyTableArea = oMySheet.ActiveArea.SplitBottom("ChannelTable",50)
oMyTableArea.DisplayObjType = "ChannelTable"
oMyTableArea.DisplayObj.DynamicMode = "All"
oMySheet.Cursor.Type = "Band"
oMySheet.Cursor.Mode = "GraphPoints"
oMyTableArea.DisplayObj.CursorMode = dd.eVIEWChannelTableHighlightRows
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_CursorMode_IToChannelTableInt.htm`*
