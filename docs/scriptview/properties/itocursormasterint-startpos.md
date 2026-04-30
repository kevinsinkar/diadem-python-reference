---
title: "IToCursorMasterInt.StartPos"
description: "Specifies the beginning of the value range in DIAdem VIEW in which DIAdem moves the cursor during play-back."
---

# IToCursorMasterInt.StartPos

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: StartPos for Cursor

Specifies the beginning of the value range in DIAdem VIEW in which DIAdem moves the cursor during play-back.

## Signature

```python
obj.StartPos
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
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_StartPos_IToCursorMasterInt.htm`*
