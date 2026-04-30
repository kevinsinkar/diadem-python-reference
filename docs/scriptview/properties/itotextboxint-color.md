---
title: "IToTextBoxInt.Color"
description: "Specifies the color of the text in a textbox in DIAdem VIEW."
---

# IToTextBoxInt.Color

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Color for TextBox

Specifies the color of the text in a textbox in DIAdem VIEW.

## Signature

```python
obj.Color
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Text = "Current time: @CurrDate@"
oMyObj.Color = "red"
oMyObj.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Generating and Formatting Text</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Color_IToTextBoxInt.htm`*
