---
title: "IToAreaObjectInt.DisplayObjType"
description: "Specifies the display type of an area in DIAdem VIEW. When the display type changes, DIAdem tries to adopt the properties of the previous object."
---

# IToAreaObjectInt.DisplayObjType

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DisplayObjType for Area

Specifies the display type of an area in DIAdem VIEW. When the display type changes, DIAdem tries to adopt the properties of the previous object.

## Signature

```python
obj.DisplayObjType
```

## Python example

```python
for viewArea in dd.VIEW.ActiveSheet.Areas:
    dd.MsgBoxDisp(viewArea.DisplayObjType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DisplayObjType_IToAreaObjectInt.htm`*
