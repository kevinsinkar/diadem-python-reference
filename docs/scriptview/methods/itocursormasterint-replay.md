---
title: "IToCursorMasterInt.Replay"
description: "Moves the cursor automatically along the enabled curve in the enabled area, or plays the video in the enabled area in DIAdem VIEW."
---

# IToCursorMasterInt.Replay

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: Replay for Cursor

Moves the cursor automatically along the enabled curve in the enabled area, or plays the video in the enabled area in DIAdem VIEW.

## Signature

```python
obj.Replay(Sequential)
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
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_Replay_IToCursorMasterInt.htm`*
