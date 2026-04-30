---
title: "IToFontInt"
description: "The Font object provides access to the font in a textbox or in a channel table in DIAdem VIEW. In the Font object, you specify or request the font, the font sty"
---

# IToFontInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Font

The Font object provides access to the font in a textbox or in a channel table in DIAdem VIEW. In the Font object, you specify or request the font, the font style, and the font size.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = oMySheet.ActiveArea.DisplayObj
OMyFont = oMyObj.Font
OMyFont.Name = "Arial"
OMyFont.Size = 48
oMyObj.BkColor = "violet"
oMyObj.Color = "black"
oMyObj.Text = "Current date: @CurrDate@"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itofontint-bold/">Bold</a> | <a href="../../properties/itofontint-italic/">Italic</a> | <a href="../../properties/itofontint-name/">Name</a> | <a href="../../properties/itofontint-size/">Size</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itochanneltableint/">ChannelTable</a>.<a href="../../properties/itochanneltableint-font/">Font</a> | <a href="../itotextboxint/">TextBox</a>.<a href="../../properties/itotextboxint-font/">Font</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Generating and Formatting Text</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToFontInt.htm`*
