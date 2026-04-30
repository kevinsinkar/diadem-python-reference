---
title: "IToAreaObjectInt.GetSize"
description: "Specifies in DIAdem VIEW the margins between an area and the edges of the worksheet, as a percentage of the size of the worksheet."
---

# IToAreaObjectInt.GetSize

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: GetSize for Area

Specifies in DIAdem VIEW the margins between an area and the edges of the worksheet, as a percentage of the size of the worksheet.

## Signature

```python
obj.GetSize(Top, Bottom, Left, Right)
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("")
oMyArea = oMySheet.ActiveArea
oMyTopArea = oMyArea.SplitTop("TopArea", 0.5)
oMyRightArea = oMyTopArea.SplitRight("RightArea", 0.5)
oMyBottomArea = oMyRightArea.SplitBottom("BottomArea", 0.5)
oMyLeftArea = oMyBottomArea.SplitLeft("LeftArea", 0.5)
oMyLeftArea.GetSize(dTop, dBottom, dRight, dLeft)
dd.MsgBoxDisp("Top: " + dTop + ", " + "Bottom: " + dBottom + "\r\n" + "Left: " + dLeft + ", " + "Right: " + dRight)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_GetSize_IToAreaObjectInt.htm`*
