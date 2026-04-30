---
title: "IToCursorMasterInt.XRangeMode"
description: "Specifies how DIAdem VIEW determines the start value and the end value for the methods GotoStart and GotoEnd ."
---

# IToCursorMasterInt.XRangeMode

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: XRangeMode for Cursor

Specifies how DIAdem VIEW determines the start value and the end value for the methods GotoStart and GotoEnd .

## Signature

```python
obj.XRangeMode
```

## Python example

```python
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Video"
oMySheet.ActiveArea.DisplayObj.FileName = dd.ProgramDrv  + "\\Examples\\Documents\\Austin_Drive.wmv"
oMySheet.Cursor.XRangeMode = "automatic"
oMySheet.Cursor.GotoStart()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_XRangeMode_IToCursorMasterInt.htm`*
