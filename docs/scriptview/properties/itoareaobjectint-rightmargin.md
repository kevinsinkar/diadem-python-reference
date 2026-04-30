---
title: "IToAreaObjectInt.RightMargin"
description: "Returns the distance of an area to the right edge of a worksheet in DIAdem VIEW as a percentage."
---

# IToAreaObjectInt.RightMargin

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: RightMargin for Area

Returns the distance of an area to the right edge of a worksheet in DIAdem VIEW as a percentage.

## Signature

```python
obj.RightMargin
```

## Python example

```python
oMyArea = dd.View.ActiveSheet.ActiveArea
dd.MsgBoxDisp("Top: " + oMyArea.TopMargin + "\r\n" + "Left: " + oMyArea.LeftMargin + "\r\n" +"Right: " + oMyArea.RightMargin + "\r\n" + "Bottom: " + oMyArea.BottomMargin)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_RightMargin_IToAreaObjectInt.htm`*
