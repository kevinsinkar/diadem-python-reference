---
title: "IToTextBoxInt.BkColorRGB"
description: "Specifies the background color of a text in a textbox in DIAdem VIEW. The color is only used when the BkColor property has the value other colors ."
---

# IToTextBoxInt.BkColorRGB

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: BkColorRGB for TextBox

Specifies the background color of a text in a textbox in DIAdem VIEW. The color is only used when the BkColor property has the value other colors .

## Signature

```python
obj.BkColorRGB
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Use the VBS function <span class="Monospace">RGB</span> to calculate the RGB value of colors, based on the proportions of red, green, and blue.</td></tr>
</table>
</div>

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Text = "Current time: @CurrDate@"
oMyObj.BkColor = "other colors"
oMyObj.BkColorRGB = dd.RGB(0,0,255)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Generating and Formatting Text</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_BkColorRGB_IToTextBoxInt.htm`*
