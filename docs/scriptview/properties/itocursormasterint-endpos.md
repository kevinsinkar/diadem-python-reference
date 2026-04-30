---
title: "IToCursorMasterInt.EndPos"
description: "Specifies in DIAdem VIEW the end of the value range in which DIAdem moves the cursor during playback."
---

# IToCursorMasterInt.EndPos

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: EndPos for Cursor

Specifies in DIAdem VIEW the end of the value range in which DIAdem moves the cursor during playback.

## Signature

```python
obj.EndPos
```

## Python example

```python
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Video"
oMySheet.ActiveArea.DisplayObj.FileName = dd.ProgramDrv  + "\\Examples\\Documents\\Austin_Drive.wmv"
oMySheet.Cursor.XRangeMode = "manual"
oMySheet.Cursor.StartPos = 50
oMySheet.Cursor.EndPos = 250
oMySheet.Cursor.GotoStart()
oMySheet.Cursor.Play()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring a Map Display</a> | <a href="#" data-unresolved="1">Configuring a Text Box Display</a> | <a href="#" data-unresolved="1">Deleting Curve Sections and Interpolating over Specified Points</a> | <a href="#" data-unresolved="1">Displaying 2D Axis Systems with Several Y-Axes</a> | <a href="#" data-unresolved="1">Displaying Images in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Displaying Properties in the Legend of a Curve</a> | <a href="#" data-unresolved="1">Displaying the Curve Coordinates</a> | <a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a> | <a href="#" data-unresolved="1">Finding Values in Channel Tables</a> | <a href="#" data-unresolved="1">Interpolating Curve Points</a> | <a href="#" data-unresolved="1">Setting the Leading Curve</a> | <a href="#" data-unresolved="1">Transferring VIEW Layouts to DIAdem REPORT</a> | <a href="#" data-unresolved="1">Viewing Data as Curves</a> | <a href="#" data-unresolved="1">Zooming and Scrolling Curve Areas</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_EndPos_IToCursorMasterInt.htm`*
