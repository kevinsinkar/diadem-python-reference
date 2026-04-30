---
title: "IToCursorMasterInt.IsPlaying"
description: "Specifies whether the cursor moves automatically along the active curve in the active area, or whether the video runs in the active area."
---

# IToCursorMasterInt.IsPlaying

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: IsPlaying for Cursor

Specifies whether the cursor moves automatically along the active curve in the active area, or whether the video runs in the active area.

## Signature

```python
bIsPlaying = Object.IsPlaying()
```

## Python example

```python
dd.View.Events.OnCursorChanged = "DisplayCursor"
```

```python
def DisplayCursor(oCursor):
    if oCursor.IsPlaying :
        Text = Text + "Mode : " + oCursor.Mode + "\r\n"
        Text = Text + "Type : " + oCursor.Type + "\r\n"
        Text = Text + "X1   : " + oCursor.X1 + "\r\n"
        Text = Text + "Y1   : " + oCursor.Y1 + "\r\n"
        Text = Text + "X2   : " + oCursor.X2 + "\r\n"
        Text = Text + "Y2   : " + oCursor.Y2 + "\r\n"
        Text = Text + "dX   : " + oCursor.dX + "\r\n"
        Text = Text + "dY   : " + oCursor.dY + "\r\n"
        Text = Text + "P1   : " + oCursor.P1 + "\r\n"
        Text = Text + "P2   : " + oCursor.P2 + "\r\n"
        oCursor.Sheet.Areas(2).DisplayObj.Text = Text
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_IsPlaying_IToCursorMasterInt.htm`*
