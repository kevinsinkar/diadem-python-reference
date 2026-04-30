---
title: "IToColorPaletteEntryInt"
description: "The ColorPaletteEntry object provides access to a color palette entry in a contour or a bird's eye view display in DIAdem VIEW."
---

# IToColorPaletteEntryInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: ColorPaletteEntry

The ColorPaletteEntry object provides access to a color palette entry in a contour or a bird's eye view display in DIAdem VIEW.

## Python example

```python
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "Contour" :
    oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj.UserDefinedColoringEntries
    for i in range( 1, oMyObj.Count+1):
        dd.LogfileWrite("Color: " + oMyObj(i).Color + ", ColorRGB: " + oMyObj(i).ColorRGB + ", Value: " + oMyObj(i).Value)
```

```python
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "BirdsEyeView" :
    oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects(1).UserDefinedColoringEntries
    for i in range( 1, oMyObj.Count+1):
        dd.LogfileWrite("Color: " + oMyObj(i).Color + ", ColorRGB: " + oMyObj(i).ColorRGB + ", Value: " + oMyObj(i).Value)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itocolorpaletteentryint-color/">Color</a> | <a href="../../properties/itocolorpaletteentryint-colorrgb/">ColorRGB</a> | <a href="../../properties/itocolorpaletteentryint-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/colorpaletteentries/">ColorPaletteEntries</a>.<a href="../../methods/itocolorpaletteentriesint-add/">Add</a> | <a href="../../collections/colorpaletteentries/">ColorPaletteEntries</a>.<a href="../../methods/itocolorpaletteentriesint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToColorPaletteEntryInt.htm`*
