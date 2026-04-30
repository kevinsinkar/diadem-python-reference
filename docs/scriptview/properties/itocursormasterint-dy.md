---
title: "IToCursorMasterInt.DY"
description: "Returns the distance between the upper and the lower cursor for the frame cursor in DIAdem VIEW."
---

# IToCursorMasterInt.DY

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DY for Cursor

Returns the distance between the upper and the lower cursor for the frame cursor in DIAdem VIEW.

## Signature

```python
obj.DY
```

## Python example

```python
dd.View.sheets(1).Cursor.Type = "Frame"
dd.View.CoordinateWnd.Visible = True
dd.View.ActiveSheet.Cursor.X1 = 10
dd.View.ActiveSheet.Cursor.Y1 = 20
dd.View.ActiveSheet.Cursor.X2 = 30
dd.View.ActiveSheet.Cursor.Y2 = 40
dd.MsgBoxDisp("DX position: " + dd.View.ActiveSheet.Cursor.DX + "\r\n" + "DY position: " + dd.View.ActiveSheet.Cursor.DY)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Analyzing and Displaying Channels Section by Section</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Background Segments in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Show texts of assignment channels in the VIEW legend</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DY_IToCursorMasterInt.htm`*
