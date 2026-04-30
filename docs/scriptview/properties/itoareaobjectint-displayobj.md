---
title: "IToAreaObjectInt.DisplayObj"
description: "Returns the Dialog object in an area in DIAdem VIEW."
---

# IToAreaObjectInt.DisplayObj

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DisplayObj for Area

Returns the Dialog object in an area in DIAdem VIEW.

## Signature

```python
return_value = obj.DisplayObj
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "TextBox"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.Text= "Current time: @CurrDate@"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DisplayObj_IToAreaObjectInt.htm`*
