---
title: "IToCursorMasterInt"
description: "The Cursor object provides a cursor in DIAdem VIEW. You use the Cursor object to specify the cursor position, the cursor type, and the cursor mode. You can set "
---

# IToCursorMasterInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Cursor

The Cursor object provides a cursor in DIAdem VIEW. You use the Cursor object to specify the cursor position, the cursor type, and the cursor mode. You can set the Cursor object separately for each worksheet.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "CurveChart2D"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.Curves2D.Add("[1]/[1]","[1]/[2]")
oMySheet.Cursor.Type = "Frame"
oMySheet.Cursor.X1 = 10
oMySheet.Cursor.Y1 = 20
oMySheet.Cursor.X2 = 30
oMySheet.Cursor.Y2 = 40
dd.LogFileWrite("Dx position: " + dd.View.ActiveSheet.Cursor.Dx + "\r\n" + "Dy position: " + dd.View.ActiveSheet.Cursor.Dy)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itocursormasterint-activecursorcolorrgb/">ActiveCursorColorRGB</a> | <a href="../../properties/itocursormasterint-constantdeltas/">ConstantDeltas</a> | <a href="../../properties/itocursormasterint-cursorwidth/">CursorWidth</a> | <a href="../../properties/itocursormasterint-dimensions/">Dimensions</a> | <a href="../../properties/itocursormasterint-dx/">DX</a> | <a href="../../properties/itocursormasterint-dy/">DY</a> | <a href="../../properties/itocursormasterint-endpos/">EndPos</a> | <a href="../../properties/itocursormasterint-hotspotcolorrgb/">HotspotColorRGB</a> | <a href="../../properties/itocursormasterint-inactivecursorcolorrgb/">InactiveCursorColorRGB</a> | <a href="../../properties/itocursormasterint-interpolating/">Interpolating</a> | <a href="../../properties/itocursormasterint-mode/">Mode</a> | <a href="../../properties/itocursormasterint-p1/">P1</a> | <a href="../../properties/itocursormasterint-p2/">P2</a> | <a href="../../properties/itocursormasterint-sheet/">Sheet</a> | <a href="../../properties/itocursormasterint-speed/">Speed</a> | <a href="../../properties/itocursormasterint-startpos/">StartPos</a> | <a href="../../properties/itocursormasterint-subcursor/">SubCursor</a> | <a href="../../properties/itocursormasterint-type/">Type</a> | <a href="../../properties/itocursormasterint-x1/">X1</a> | <a href="../../properties/itocursormasterint-x2/">X2</a> | <a href="../../properties/itocursormasterint-xrangemode/">XRangeMode</a> | <a href="../../properties/itocursormasterint-y1/">Y1</a> | <a href="../../properties/itocursormasterint-y2/">Y2</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itocursormasterint-backwards/">Backwards</a> | <a href="../../methods/itocursormasterint-forwards/">Forwards</a> | <a href="../../methods/itocursormasterint-gotoend/">GotoEnd</a> | <a href="../../methods/itocursormasterint-gotostart/">GotoStart</a> | <a href="../../methods/itocursormasterint-isplaying/">IsPlaying</a> | <a href="../../methods/itocursormasterint-play/">Play</a> | <a href="../../methods/itocursormasterint-replay/">Replay</a> | <a href="../../methods/itocursormasterint-stepbackwards/">StepBackwards</a> | <a href="../../methods/itocursormasterint-stepforwards/">StepForwards</a> | <a href="../../methods/itocursormasterint-stop/">Stop</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itocoordinatedisplayint/">CoordinateWnd</a>.<a href="../../properties/itocoordinatedisplayint-cursor/">Cursor</a> | <a href="../itosheetint/">Sheet</a>.<a href="../../properties/itosheetint-cursor/">Cursor</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Analyzing and Displaying Channels Section by Section</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Background Segments in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Show texts of assignment channels in the VIEW legend</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToCursorMasterInt.htm`*
