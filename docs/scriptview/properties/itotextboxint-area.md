---
title: "IToTextBoxInt.Area"
description: "Returns the area in DIAdem VIEW that contains a textbox."
---

# IToTextBoxInt.Area

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Area for TextBox

Returns the area in DIAdem VIEW that contains a textbox.

## Signature

```python
return_value = obj.Area
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "TextBox"
oMyDisplayObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyDisplayObj.Text = "Hello"
dd.MsgBoxDisp("Name " + oMyDisplayObj.Area.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Area_IToTextBoxInt.htm`*
