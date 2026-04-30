---
title: "IToCursorMasterInt.Speed"
description: "Specifies the speed for the cursor in DIAdem VIEW."
---

# IToCursorMasterInt.Speed

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Speed for Cursor

Specifies the speed for the cursor in DIAdem VIEW.

## Signature

```python
obj.Speed
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "CurveChart2D"
oMyObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyObj.Curves2D.Add("[1]/[1]","[1]/[3]")
oMyCursor = dd.View.ActiveSheet.Cursor
oMyCursor.Type = "Crosshair"
oMyCursor.Speed = 10
dd.WndShow ("VIEW")
oMyCursor.GotoStart()
oMyCursor.Play(False)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Speed_IToCursorMasterInt.htm`*
