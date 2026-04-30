---
title: "IToAreaObjectInt.SplitLeft"
description: "Creates a new area and splits the specified area in DIAdem VIEW. The new area is created to the left of the active area."
---

# IToAreaObjectInt.SplitLeft

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: SplitLeft for Area

Creates a new area and splits the specified area in DIAdem VIEW. The new area is created to the left of the active area.

## Signature

```python
return_value = obj.SplitLeft(Name, Ratio)
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewSheet")
oMyArea = oMySheet.ActiveArea
oMyTopArea = oMyArea.SplitTop("TopArea",0.5)
oMyRightArea = oMyTopArea.SplitRight("RightArea",0.5)
oMyBottomArea = oMyRightArea.SplitBottom("BottomArea",0.5)
oMyLeftArea = oMyBottomArea.SplitLeft("LeftArea",0.5)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_SplitLeft_IToAreaObjectInt.htm`*
