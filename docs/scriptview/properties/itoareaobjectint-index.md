---
title: "IToAreaObjectInt.Index"
description: "Returns the index of an area in DIAdem VIEW."
---

# IToAreaObjectInt.Index

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Index for Area

Returns the index of an area in DIAdem VIEW.

## Signature

```python
obj.Index
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.SplitRight("MyArea",0.5)
dd.MsgBoxDisp("Index of MyArea: " + dd.View.ActiveSheet.Areas("MyArea").Index)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Index_IToAreaObjectInt.htm`*
