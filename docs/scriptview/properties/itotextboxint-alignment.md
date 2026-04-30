---
title: "IToTextBoxInt.Alignment"
description: "Specifies the alignment of a text in a textbox in DIAdem VIEW."
---

# IToTextBoxInt.Alignment

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Alignment for TextBox

Specifies the alignment of a text in a textbox in DIAdem VIEW.

## Signature

```python
obj.Alignment
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Text = "Current time: @CurrDate@"
oMyObj.Alignment = "Center"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Alignment_IToTextBoxInt.htm`*
