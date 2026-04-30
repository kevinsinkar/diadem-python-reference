---
title: "IToCursorMasterInt.Stop"
description: "Stops the cursor movement automatically along the enabled curve in the enabled area, or stops the video in the enabled area."
---

# IToCursorMasterInt.Stop

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: Stop for Cursor

Stops the cursor movement automatically along the enabled curve in the enabled area, or stops the video in the enabled area.

## Signature

```python
obj.Stop()
```

## Python example

```python
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Video"
oMySheet.ActiveArea.DisplayObj.FileName = dd.ProgramDrv  + "\\Examples\\Documents\\Austin_Drive.wmv"
oMySheet.Cursor.XRangeMode = "automatic"
oMySheet.Cursor.GotoStart()
dd.WndOpen("VIEW")
oMySheet.Cursor.RePlay(False)
dd.MsgBoxDisp("Stop")
oMySheet.Cursor.Stop()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">3D Interpolation</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Recording Video and Measurement Data</a> | <a href="#" data-unresolved="1">Synchronizing Maps, Videos, and Measurement Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_Stop_IToCursorMasterInt.htm`*
