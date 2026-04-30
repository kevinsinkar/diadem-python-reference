---
title: "ITDMModelEnumerations.Item"
description: "Returns in the model of a data store the enumeration belonging to a specific index or to a specific definition. Note You can always omit the Item method because"
---

# ITDMModelEnumerations.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for ModelEnumerations

Returns in the model of a data store the enumeration belonging to a specific index or to a specific definition. Note You can always omit the Item method because it is the standard element of the collection.

## Signature

```python
return_value = obj.Item(IndexOrDefinition)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyEnums = oMyDataStore.Model.Enumerations
print(oMyEnums.Item(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_ITDMModelEnumerations.htm`*
