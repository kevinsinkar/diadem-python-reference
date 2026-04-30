---
title: "IToCursorMasterInt.HotspotColorRGB"
description: "Specifies the color of the small square with which DIAdem marks the intersection point of the cursor lines in DIAdem VIEW. Use a RGB value or a VBS color consta"
---

# IToCursorMasterInt.HotspotColorRGB

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: HotspotColorRGB for Cursor

Specifies the color of the small square with which DIAdem marks the intersection point of the cursor lines in DIAdem VIEW. Use a RGB value or a VBS color constant to specify the color.

## Signature

```python
obj.HotspotColorRGB
```

## Python example

```python
oMyCursor = dd.View.ActiveSheet.Cursor
oMyCursor.Type = "Crosshair"
oMyCursor.ActiveCursorColorRGB = dd.RGB(255, 0, 0)
oMyCursor.InactiveCursorColorRGB = dd.RGB(0, 0, 255)
oMyCursor.HotspotColorRGB = 0
oMyCursor.CursorWidth = 3
```

## See also

<div markdown="1">
<div class="SeeAlso">
<p class="body">The following example sets the type, the color, and the line width of the cursor:</p><table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div><div class="codeblue"><pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMyCursor
<span class="HlVBSKeyword">Set</span> oMyCursor = <span class="Hldiademobject">View.ActiveSheet.Cursor</span>
oMyCursor.Type = <span class="HlString">"Crosshair"</span>
oMyCursor.ActiveCursorColorRGB = <span class="HlVBSKeyword"><span class="Hldiademcommand">RGB</span></span>(<span class="HlNumbers">255</span>, <span class="HlNumbers">0</span>, <span class="HlNumbers">0</span>)
oMyCursor.InactiveCursorColorRGB = <span class="HlVBSKeyword"><span class="Hldiademcommand">RGB</span></span>(<span class="HlNumbers">0</span>, <span class="HlNumbers">0</span>, <span class="HlNumbers">255</span>)
oMyCursor.HotspotColorRGB = <span class="HlVBSKeyword">VBBlack</span>
oMyCursor.CursorWidth = <span class="HlNumbers">3</span></donottranslate></pre></div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>oMyCursor = dd.View.ActiveSheet.Cursor 
oMyCursor.Type = <span class="HlString">"Crosshair"</span> 
oMyCursor.ActiveCursorColorRGB = dd.RGB(<span class="HlNumbers">255</span>, <span class="HlNumbers">0</span>, <span class="HlNumbers">0</span>) 
oMyCursor.InactiveCursorColorRGB = dd.RGB(<span class="HlNumbers">0</span>, <span class="HlNumbers">0</span>, <span class="HlNumbers">255</span>) 
oMyCursor.HotspotColorRGB = <span class="HlNumbers">0</span> 
oMyCursor.CursorWidth = <span class="HlNumbers">3</span> </donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_HotspotColorRGB_IToCursorMasterInt.htm`*
