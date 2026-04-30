---
title: "IToTextBoxInt.Font"
description: "Returns the settings for the font in a textbox in DIAdem VIEW."
---

# IToTextBoxInt.Font

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Font for TextBox

Returns the settings for the font in a textbox in DIAdem VIEW.

## Signature

```python
return_value = obj.Font
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Text = "Current time: @CurrDate@"
oMyObj.Font.Name = "Arial"
oMyObj.Font.Size = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Font_IToTextBoxInt.htm`*
