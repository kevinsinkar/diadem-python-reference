---
title: "IToFontInt.Name"
description: "Specifies the name of the font in a textbox in DIAdem VIEW."
---

# IToFontInt.Name

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Name for Font

Specifies the name of the font in a textbox in DIAdem VIEW.

## Signature

```python
obj.Name
```

## Python example

```python
if dd.View.ActiveSheet.ActiveArea.DisplayObjType == "TextBox" :
    oMyText = dd.View.ActiveSheet.ActiveArea.DisplayObj
    dd.MsgBoxDisp("Font: " + oMyText.Font.Name + ", " + oMyText.Font.Size + "\r\n" + "Bold:   " + oMyText.Font.Bold + "\r\n" + "Italic: " + oMyText.Font.Italic)
else:
    dd.MsgBoxDisp("Area type: " + dd.View.ActiveSheet.ActiveArea.DisplayObjType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Generating and Formatting Text</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Name_IToFontInt.htm`*
