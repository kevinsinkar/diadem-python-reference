---
title: "ColorPaletteEntries"
description: "The ColorPaletteEntries object provides a collection of user-defined colors of a contour or a bird's eye view display in DIAdem VIEW. Use the ColorPaletteEntrie"
---

# ColorPaletteEntries

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: ColorPaletteEntries

The ColorPaletteEntries object provides a collection of user-defined colors of a contour or a bird's eye view display in DIAdem VIEW. Use the ColorPaletteEntries collection to delete palette colors or to add new colors to the palette.

## Python example

```python
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj.CurvesContour(1).UserDefinedColoringEntries
for i in range( 1, oMyObj.Count+1):
    dd.LogfileWrite("Color: " + oMyObj(i).Color + " / Value: " + oMyObj(i).Value)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itocolorpaletteentriesint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itocolorpaletteentriesint-add/">Add</a> | <a href="../../methods/itocolorpaletteentriesint-item/">Item</a> | <a href="../../methods/itocolorpaletteentriesint-remove/">Remove</a> | <a href="../../methods/itocolorpaletteentriesint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itobirdseyeviewobjectint/">BirdsEyeViewDynamicObject</a>.<a href="../../properties/itobirdseyeviewobjectint-userdefinedcoloringentries/">UserDefinedColoringEntries</a> | <a href="../../objects/itocontourcurveint/">ContourCurve</a>.<a href="../../properties/itocontourcurveint-userdefinedcoloringentries/">UserDefinedColoringEntries</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToColorPaletteEntriesInt.htm`*
