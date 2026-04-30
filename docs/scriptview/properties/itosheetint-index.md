---
title: "IToSheetInt.Index"
description: "Returns the index of a worksheet in DIAdem VIEW. The index corresponds to the display position in DIAdem VIEW."
---

# IToSheetInt.Index

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Index for Sheet

Returns the index of a worksheet in DIAdem VIEW. The index corresponds to the display position in DIAdem VIEW.

## Signature

```python
obj.Index
```

## Python example

```python
dd.View.Sheets.Add("MySheet")
dd.MsgBoxDisp("Index of MySheet: " + dd.View.Sheets("MySheet").Index)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Index_IToSheetInt.htm`*
