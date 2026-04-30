---
title: "IToTextBoxInt.BkColor"
description: "Specifies the background color of a text in a textbox in DIAdem VIEW."
---

# IToTextBoxInt.BkColor

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: BkColor for TextBox

Specifies the background color of a text in a textbox in DIAdem VIEW.

## Signature

```python
obj.BkColor
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Text = "Current time: @CurrDate@"
oMyObj.BkColor = "red"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Generating and Formatting Text</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_BkColor_IToTextBoxInt.htm`*
