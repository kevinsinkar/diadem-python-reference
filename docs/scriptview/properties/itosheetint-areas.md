---
title: "IToSheetInt.Areas"
description: "Returns the Areas collection in DIAdem VIEW."
---

# IToSheetInt.Areas

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Areas for Sheet

Returns the Areas collection in DIAdem VIEW.

## Signature

```python
return_value = obj.Areas
```

## Python example

```python
for oMyArea in dd.View.ActiveSheet.Areas:
    dd.MsgBoxDisp("Type of area: " + oMyArea.DisplayObjType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Areas_IToSheetInt.htm`*
